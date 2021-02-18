
Now, let's restore the application. 

First, let's delete the app. This will delete the entire app and PVCs.

`kubectl delete ns demo`{{execute}}

After the delete completes, head over the app and check it is not available.

https://[[HOST2_SUBDOMAIN]]-30123-[[KATACODA_HOST]].environments.katacoda.com

Next, head over to the backup UI and find your backup.

Select the backup using the right three dots and click restore.

1. Give your restore a name.
2. Select the `katacoda-px` cluster in desitnation cluster list.
3. Select `Replace existing resources`

Verify your backup has completed. It will turn green in the backup UI. 

Then waiting for the application to come back online and see your data is recovered. Note, it can take up to 5 minutes for the UI to come back on Katacoda.

`watch kubectl get po -n demo`{{execute}}

When its running again, head over to the app again, your data should be there.

https://[[HOST2_SUBDOMAIN]]-30123-[[KATACODA_HOST]].environments.katacoda.com
