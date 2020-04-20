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
