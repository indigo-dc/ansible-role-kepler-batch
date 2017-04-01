FROM indigodatacloud/ubuntu-sshd:14.04
MAINTAINER Mario David <mariojmdavid@gmail.com>
LABEL description="Container image to run Kepler WF engine"

RUN ansible-galaxy install indigo-dc.kepler-batch && \
    ansible-playbook /etc/ansible/roles/indigo-dc.kepler-batch/tests/kepler.yml

USER indigo
ENV FUTUREGATEWAY_URI 'set_this_when_running_docker'
ENV AUTHORIZATION_TOKEN 'set_this_when_running_docker'
ENV CONFIG_JSON '[{"host":"","port":"","login":"","password":"","argument":""}]'
CMD echo $CONFIG_JSON > /home/indigo/ophidia/ensemble-visualization/phase1/config.json && \
    /usr/local/Kepler-2.5/kepler.sh -runwf -nogui /usr/local/indigokepler/workflows/ophidia/ensemble-visualization/OphidiaEnsembleAnalysisVisualization.kar
