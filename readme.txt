git remote add origin https://github.com/hainagmca/pal-tracker-distributed.git
git cherry-pick pipeline

https://github.com/hainagmca/pal-tracker-distributed/settings/secrets

CF_API_URL=api.run.pivotal.io

CF_ORG=DellEMC_PAL

CF_SPACE=Nagendra.Chunduru@emc.com

CF_USERNAME=nagendra.chunduru@dell.com

CF_PASSWORD

cd ~/workspace/assignment-submission
./gradlew cloudNativeDeveloperDistributedSystemDeployment \
    -PregistrationServerUrl=https://registration-pal-nag-covid.cfapps.io \
    -PbacklogServerUrl=https://backlog-pal-nag-covid.cfapps.io \
    -PallocationsServerUrl=https://allocations-pal-nag-covid.cfapps.io \
    -PtimesheetsServerUrl=https://timesheets-pal-nag-covid.cfapps.io


=======================================================================================================

C:\LABs\Aug CND\assignment-submission>gradlew cloudNativeDeveloperDistributedSystemWithSecurity     -PuaaUrl=https://p-identity.login.sys.evans.pal.pivotal.io     -PclientId=a555a8ca-c465-462c-8737-445665d4bbc0     -PclientSecret=ca2d48ce-0d1b-439c-820a-55f6aab825e0     -PregistrationServerUrl=https://registration-pal-nag-wipro.apps.evans.pal.pivotal.io  -PbacklogServerUrl=https://backlog-pal-nag-wipro.apps.evans.pal.pivotal.io     -PallocationsServerUrl=https://allocations-pal-nag-wipro.apps.evans.pal.pivotal.io     -PtimesheetsServerUrl=https://timesheets-pal-nag-wipro.apps.evans.pal.pivotal.io

> Task :cloudNativeDeveloperDistributedSystemWithSecurity

Starting assignment...

GET https://registration-pal-nag-wipro.apps.evans.pal.pivotal.io/
GET https://registration-pal-nag-wipro.apps.evans.pal.pivotal.io/actuator/env
GET https://backlog-pal-nag-wipro.apps.evans.pal.pivotal.io/
GET https://backlog-pal-nag-wipro.apps.evans.pal.pivotal.io/actuator/env
GET https://allocations-pal-nag-wipro.apps.evans.pal.pivotal.io/
GET https://allocations-pal-nag-wipro.apps.evans.pal.pivotal.io/actuator/env
GET https://timesheets-pal-nag-wipro.apps.evans.pal.pivotal.io/
GET https://timesheets-pal-nag-wipro.apps.evans.pal.pivotal.io/actuator/env
POST https://p-identity.login.sys.evans.pal.pivotal.io/oauth/token
POST https://registration-pal-nag-wipro.apps.evans.pal.pivotal.io/registration
POST https://p-identity.login.sys.evans.pal.pivotal.io/oauth/token
GET https://registration-pal-nag-wipro.apps.evans.pal.pivotal.io/accounts?ownerId=1
POST https://p-identity.login.sys.evans.pal.pivotal.io/oauth/token
POST https://registration-pal-nag-wipro.apps.evans.pal.pivotal.io/projects
POST https://p-identity.login.sys.evans.pal.pivotal.io/oauth/token
POST https://allocations-pal-nag-wipro.apps.evans.pal.pivotal.io/allocations
POST https://p-identity.login.sys.evans.pal.pivotal.io/oauth/token
POST https://backlog-pal-nag-wipro.apps.evans.pal.pivotal.io/stories
POST https://p-identity.login.sys.evans.pal.pivotal.io/oauth/token
POST https://timesheets-pal-nag-wipro.apps.evans.pal.pivotal.io/time-entries

Assignment was successful.


BUILD SUCCESSFUL in 23s
1 actionable task: 1 executed
C:\LABs\Aug CND\assignment-submission>


=========================================================================================================
