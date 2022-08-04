# governance-best-practises-for-apps

repository showing best practices for apps

Based on the following links:

* https://cloud.redhat.com/blog/9-best-practices-for-deploying-highly-available-applications-to-openshift
* https://cloud.redhat.com/blog/14-best-practices-for-developing-applications-on-openshift

we look to create a PolicySet based on RHACM-Policies and Kyverno Integration


## How to run it
```shell
oc apply -f https://raw.githubusercontent.com/ch-stark/governance-best-practises-for-apps/main/setup/openshift-gitops
oc apply -f https://raw.githubusercontent.com/ch-stark/governance-best-practises-for-apps/main/setup/rhacm-policies
until oc apply -f https://raw.githubusercontent.com/ch-stark/governance-best-practises-for-apps/main/setup/rhacm-policies; do sleep 15; done
```




