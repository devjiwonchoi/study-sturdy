- Immutable Deployment policy
	- ensures that your new application version is always deployed to new instances, instead of updating existing instances.
	- quick and safe rollback in case the deployment fails.
	- a second Auto Scaling group is launched in your environment and the new version serves traffic alongside the old version until the new instances pass health checks.
	- In case of deployment failure, the new instances are terminated
- All at once
	- 'All at once' is the quickest deployment method, but the application may become unavailable to users (or have low availability) for a short time.
- Rolling
	- avoids downtime and minimizes reduced availability, at a cost of a longer deployment time
	- in case of deployment failure, the rollback process is via manual redeploy
	- with additional batch
		- 