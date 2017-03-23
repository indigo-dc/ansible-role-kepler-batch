FROM indigodatacloud/ubuntu-sshd:14.04
MAINTAINER Mario David <mariojmdavid@gmail.com>
LABEL description="Container image to run Kepler WF engine"

RUN ansible-galaxy install indigo-dc.kepler-batch && \
    ansible-playbook /etc/ansible/roles/indigo-dc.kepler-batch/tests/kepler.yml

USER indigo
ENV CONFIG_JSON '[{"host":"","port":"","login":"","password":"","argument":""}]'
CMD echo $CONFIG_JSON > /home/indigo/ophidia/ensemble-visualization/phase1/config.json && \
    /usr/local/Kepler-2.5/kepler.sh -runwf -nogui /usr/local/Kepler-2.5/outreach-2.4.0/workflows/demos/getting-started/04-HelloWorld.xml
