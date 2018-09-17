# Release Instructions

1. Update versions for release
    - Change the [VERSION](./VERSION) file to drop the ".dev0"
    - Update `nupic.core` version in [bindings/py/requirements.txt](/bindings/py/requirements.txt) to the latest
    - Merge `release` version changes to master
2. Deploy
    - Run the deployment project in [Bamboo](https://ci.numenta.com/deploy/viewDeploymentProjectEnvironments.action?id=63078401) for the build that includes the version change
    - Check if the new version was deployed to [PyPi](https://pypi.org/project/htmresearch-core/)
    - Create a release in [Github](https://github.com/numenta/htmresearch-core/releases) using the new version as the title
3. Update versions for development
    - Bump the version in the [VERSION](./VERSION) file and add the ".dev0" extension
    - Merge `dev` version changes to master
