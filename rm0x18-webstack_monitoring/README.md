# Webstack monitoring
DevOps
SysAdmin
monitoring

## Concepts
For this project, look at these concepts:

[Monitoring](https://intranet.alxswe.com/concepts/13)
[Server](https://intranet.alxswe.com/concepts/67)


## Background Context
“You cannot fix or improve what you cannot measure” is a famous saying in the Tech industry. In the age of the data-ism, monitoring how our Software systems are doing is an important thing. In this project, we will implement one of many tools to measure what is going on our servers.

Web stack monitoring can be broken down into 2 categories:

Application monitoring: getting data about your running software and making sure it is behaving as expected
Server monitoring: getting data about your virtual or physical server and making sure they are not overloaded (could be CPU, memory, disk or network overload).

### Tasks
| Task | File |
| ---- | ---- |
| 0. Sign up for Datadog and install datadog-agent | [0x18-webstack_monitoring](./0x18-webstack_monitoring) |
| 1. Monitor some metrics |  |
| 2. Create a dashboard | [2-setup_datadog](./2-setup_datadog) |

### Steps
0. Sign up for Datadog and install datadog-agent

For this task head to [https://www.datadoghq.com/](https://intranet.alxswe.com/rltoken/Ufs6rTHMET5LB1Uoylx0nw) and sign up for a free Datadog account. When signing up, you’ll have the option of selecting statistics from your current stack that Datadog can monitor for you. Once you have an account set up, follow the instructions given on the website to install the Datadog agent.

* Sign up for Datadog - Please make sure you are using the US website of Datagog (https://app.datadoghq.com)
* Use the US1 region
* Install datadog-agent on web-01
* Create an application key
* Copy-paste in your Intranet user profile (here) your DataDog API key and your DataDog application key.
* Your server web-01 should be visible in Datadog under the host name XX-web-01
	* You can validate it by using this [API](https://intranet.alxswe.com/rltoken/5BtVPmgzhb96y7jZDGGHOQ)
	* If needed, you will need to update the hostname of your server

1. Monitor some metrics

Among the litany of data your monitoring service can report to you are system metrics. You can use these metrics to determine statistics such as reads/writes per second, which can help your company determine if/how they should scale. Set up some monitors within the Datadog dashboard to monitor and alert you of a few. You can read about the various system metrics that you can monitor here: [System Check](https://intranet.alxswe.com/rltoken/4RPOEVDTqKXuvyU4Gkj2Bw).

* Set up a monitor that checks the number of read requests issued to the device per second.
* Set up a monitor that checks the number of write requests issued to the device per second.

2. Create a dashboard

Now create a dashboard with different metrics displayed in order to get a few different visualizations.

* Create a new dashboard
* Add at least 4 widgets to your dashboard. They can be of any type and monitor whatever you’d like
* Create the answer file 2-setup_datadog which has the dashboard_id on the first line. Note: in order to get the id of your dashboard, you may need to use [Datadog’s API](https://intranet.alxswe.com/rltoken/QhlPcQqUocwWcOkZ9s4mWQ).


