Use this plugin to see the status of a test run in AWS Device farm. You can
override the default configuration with the following parameters:

* `access_key` - AWS access key ID - Optional
* `secret_key` - AWS secret access key - Optional
* `region` - AWS availability zone
* `test_project` - The name of the AWS device farm project
* `run_name` - the name of the run

## Example

The following is a sample configuration in your .drone.yml file:

```yaml
deploy:
  behavior-testing:
        image: kowalatech/drone-aws-device-farm-report
        access_key: hjwgjhgjhwe
        secret_key: werkjhwekjrhweuyiuwerbyiuweyrui
        region: us-west-2
        test_project: androidTestProject
        run_name: Run-app-release
```
