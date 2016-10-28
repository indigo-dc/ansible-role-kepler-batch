FROM indigodatacloud/ubuntu-sshd:14.04
MAINTAINER Mario David <mariojmdavid@gmail.com>
LABEL description="Container image to run Kepler WF engine"

RUN ansible-galaxy install indigo-dc.kepler && \
    ansible-playbook /etc/ansible/roles/indigo-dc.kepler/tests/kepler.yml

EXPOSE 22 5900
USER indigo
CMD /etc/init.d/vmcontext start
