FROM ansibleplaybookbundle/apb-base
MAINTAINER Ansible Playbook Bundle Community

LABEL "com.redhat.apb.version"="0.1.0"
LABEL "com.redhat.apb.spec"=\
"aWQ6IDliNzBlNmJmLTI2ZjgtNGMxZi1hNTdmLTA3NTAxMzg4YzFlOApuYW1lOiB3b3JkcHJlc3Mt\
aGEtYXBiCmltYWdlOiBhbnNpYmxlcGxheWJvb2tidW5kbGUvd29yZHByZXNzLWhhLWFwYgpkZXNj\
cmlwdGlvbjogSGlnaCBBdmFpbGFiaWxpdHkgV29yZHByZXNzIEFQQgpiaW5kYWJsZTogVHJ1ZQph\
c3luYzogb3B0aW9uYWwKbWV0YWRhdGE6IAogIGRvY3VtZW50YXRpb25Vcmw6IGh0dHBzOi8vd29y\
ZHByZXNzLm9yZy8KICBsb25nRGVzY3JpcHRpb246IEFuIGFwYiB0aGF0IGRlcGxveXMgSGlnaCBB\
dmFpbGFiaWxpdHkgV29yZHByZXNzCiAgZGVwZW5kZW5jaWVzOiBbJ3F1YXkuaW8vY29yZW9zL2V0\
Y2Q6bGF0ZXN0JywgJ3BlcmNvbmFsYWIvcGVyY29uYS14dHJhZGItY2x1c3Rlcjo1LjYnLCAnd29y\
ZHByZXNzJ10KICBkaXNwbGF5TmFtZTogV29yZHByZXNzLUhBIChBUEIpCiAgY29uc29sZS5vcGVu\
c2hpZnQuaW8vaWNvbkNsYXNzOiBpY29uLXdvcmRwcmVzcwogIApwYXJhbWV0ZXJzOiAKICAtIHJv\
b3RfcGFzc3dvcmQ6CiAgICAgIGRlZmF1bHQ6IGs4c3Bhc3N3b3JkCiAgICAgIHR5cGU6IHN0cmlu\
ZwogICAgICB0aXRsZTogZGF0YWJhc2Ugcm9vdCBwYXNzd29yZAogICAgICAKICAtIHh0cmFiYWNr\
dXBfcGFzc3dvcmQ6CiAgICAgIGRlZmF1bHQ6IGs4c3Bhc3N3b3JkCiAgICAgIHR5cGU6IHN0cmlu\
ZwogICAgICB0aXRsZTogYmFja3VwIHBhc3N3b3JkCiAgICAgIAogIC0gY2x1c3Rlcl9uYW1lOgog\
ICAgICBkZWZhdWx0OiBwZXJjb25hCiAgICAgIHR5cGU6IHN0cmluZwogICAgICB0aXRsZTogcGVy\
Y29uYSBjbHVzdGVyIG5hbWUKICAgICAgCiAgLSBkYXRhYmFzZV91c2VyOgogICAgICBkZWZhdWx0\
OiByb290CiAgICAgIHR5cGU6IHN0cmluZwogICAgICB0aXRsZTogZGF0YWJhc2UgdXNlciBuYW1l\
CiAgICAgIAogIC0gZGF0YWJhc2VfcGFzc3dvcmQ6CiAgICAgIGRlZmF1bHQ6IGs4c3Bhc3N3b3Jk\
CiAgICAgIHR5cGU6IHN0cmluZwogICAgICB0aXRsZTogZGF0YWJhc2UgdXNlciBwYXNzd29yZAog\
ICAgICAKICAtIGRhdGFiYXNlX3JlcGxpY2FzOgogICAgICBkZWZhdWx0OiAzCiAgICAgIHR5cGU6\
IGludAogICAgICB0aXRsZTogbnVtYmVyIG9mIGRhdGFiYXNlIG5vZGVzCiAgICAgIAogIC0gbWlu\
X3dvcmRwcmVzc19yZXBsaWNhczoKICAgICAgZGVmYXVsdDogNQogICAgICB0eXBlOiBpbnQKICAg\
ICAgdGl0bGU6IG1pbmltdW0gd29yZHByZXNzIHJlcGxpY2FzCiAgICAgIAogIC0gbWF4X3dvcmRw\
cmVzc19yZXBsaWNhczoKICAgICAgZGVmYXVsdDogMTAKICAgICAgdHlwZTogaW50CiAgICAgIHRp\
dGxlOiBtYXhpbXVtIHdvcmRwcmVzcyByZXBsaWNhcwogICAgICAKICAKcmVxdWlyZWQ6IAogIC0g\
Y2x1c3Rlcl9uYW1lCiAgLSBkYXRhYmFzZV91c2VyCiAgLSBkYXRhYmFzZV9yZXBsaWNhcwogIC0g\
bWluX3dvcmRwcmVzc19yZXBsaWNhcwogIC0gbWF4X3dvcmRwcmVzc19yZXBsaWNhcwogIA=="
COPY roles /opt/ansible/roles
COPY playbooks /opt/apb/actions
RUN chown -R apb /opt/{ansible,apb} \
    && chmod -R g=u /opt/{ansible,apb}

USER apb
