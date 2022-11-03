# The Keptn Show - What do you know about Keptn? With Adam Gardner
#Thekeptnshow #podcast

## Introduction
Hey, Everyone. Welcome to the first episode of The Keptn show. Today I have a special guest with me, Adam. He is working in Dynatrace in Research and Development and formerly working as an Automation Architect. I will handover  Adam to tell us about him. 

Thanks for coming to our episode as a guest, Adam. It is a great pleasure to have you here. 

**Adam:**


## A brief history of Keptn, Why it is started, What made developers to create Keptn?
Keptn started as an internal project within Dynatrace in 2018. Collect techniques and best practices. V0.0.1 was a workshop with key customers and partners.

Early versions were huge (required 16CPU / 32GB RAM / 30mins to install).
 [https://www.youtube.com/watch?v=wE-Dl-xVYgY](https://nam02.safelinks.protection.outlook.com/?url=https%3A%2F%2Fwww.youtube.com%2Fwatch%3Fv%3DwE-Dl-xVYgY&data=05%7C01%7Cvishruth.harithsa%40dynatrace.com%7Cb609b7900ac34d6c878408dabafc5c0c%7C70ebe3a35b30435d9d677716d74ca190%7C1%7C0%7C638027890291652327%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C3000%7C%7C%7C&sdata=EtEw%2F3oXx4IJdKM5fhuemn%2B8%2ByLCz2%2BW6CrI2m3TBtA%3D&reserved=0) 

V: You say it is huge, I was researching on the same and I agree with you, current version of Keptn is easy and we can set up within 3 minutes. Team has made lot of  improvements in these last 4 years and Keptn is growing really well.

## Road to become CNCF incubator
 [https://github.com/cncf/toc/blob/main/process/project_proposals.md](https://nam02.safelinks.protection.outlook.com/?url=https%3A%2F%2Fgithub.com%2Fcncf%2Ftoc%2Fblob%2Fmain%2Fprocess%2Fproject_proposals.md&data=05%7C01%7Cvishruth.harithsa%40dynatrace.com%7Cb609b7900ac34d6c878408dabafc5c0c%7C70ebe3a35b30435d9d677716d74ca190%7C1%7C0%7C638027890291652327%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C3000%7C%7C%7C&sdata=zQLWkd5xzDpmFP9rsoWiiNW53n%2F6H%2FBCksbJDYVk%2FHg%3D&reserved=0) 
CNCF Sandbox > Incubation (current)

V: It started in 2020 when Keptn has became sandbox project from a normal workshop project that is built in Dynatrace lab. Then in June 2021,  the idea to become a CNCF incubator was proposed. So early this year this also as accepted by CNCF and now Keptn is a CNCF incubator project. Yay! What to you think Keptn’s graduation from CNCF, do you have any thoughts about it? 

## Is there any other tools like Keptn out there?
There are event buses, pipeline tools, serverless platforms but nothing (that I’m aware of) that combines all of these things.
Even the eventing mechanism that Keptn relies on uses cloudevents (an OS standard) so if you want to swap Keptn core for a different event orchestrator, you could.

V: So you mean we can replace components of Keptn and use only those components in Keptn to accommodate our tools? Using cloudevents makes Keptn more compatible and effective. You said, there is no platform like Keptn, if this is the case then Keptn is one its kind, don’t you think?

## Is Keptn, only about cloud-native DevOps automation?
No, Keptn is fundamentally about making SRE best practices easier and more accessible. Think “best practices in an easy to consume way,”

V: Then, Keptn is more of a friend to SRE team, which addresses problems of SREs who deals with operational problems and an advocate of DevOps teams which helps them to build solutions and deploy the application effectively with reduced production defects.

## How Keptn can help oragnizations to reduce their MTTR and make monitoring decisions automated?
Keptn is tool and vendor agnostic. No vendor lock-in. You bring your monitoring tool and Keptn orchestrates it.
For example: ```keptn configure monitoring Prometheus``` – the Prometheus integration coder decided that when you issue that command, you should get Prom thresholds and alerts preconfigured for you.
The Dynatrace integration automatically creates management zones, dashboards and tag rules.

V: That’s wonderful! This means developers can write Keptn integrations to their service or tools and support to their own monitoring platform. Even in this case, Keptn works like a charm. Keptn is not a direct contributor for reducing MTTD or MTTR but Keptn definitely helps organisations to get there by adapting to organisation’s monitoring tool and helping the tool to have the ability to automate the releases. This is a symbiosis between monitoring tool and Keptn. Keptn is indeed a friend of SREs. 

## Is Keptn difficult to learn and implement in large scale implementation?
Keptn is flexible but it is powerful, so yes, it can be. That’s why the project is currently exploring things like the Keptn K8S lifecycle controller which will be a Kubernetes native way of doing pre and post deployment checks entirely with K8s primitives using CRDs. In other words, you kubectl apply a deployment and Keptn can automatically block the deployment if the preconditions aren’t ready (pre-checks) or rollback a deployment quality is too low (post checks). This is currently under active development and investigation so I encourage listeners to get involved.

Another new subproject is the lighthouse service. This is a standalone quality gate (so you lose the eventing mechanisms but you gain a lightweight, vendor agnostic).

V: Great to hear! That means Keptn is improving everyday. So, even I urge to the listener to go out there and contribute to Keptn because we need people like you. Not only development, you can suggest us the ideas and help in whatever way that is possible. So, Adam latest version of Keptn is 0.19.1,  *Do you think version 1.0 will be released soon and if so what can users expect from it?*  

## How best the Keptn is suited with open source monitoring tools like Prometheus? Will Keptn work better with Dynatrace?

As I say, Keptn orchestrates the tooling but doesn’t care what tooling. So if one tool offers functionality above and beyond another, you get that benefit while remaining flexible to anything new that may arrive in the future.

V: I have a small question for you, I know it is little ambitious but, Do you think if in future, Keptn gets a feature where it uses artificial intelligence for its quality gates to makes decision rather than using predefined service level indicators to pass the validation tests of the release? 

## Does Keptn supports integration with Monitoring tools like, Splunk, New relic and AppDynamics? (Discussion)
Yes. 

In this case,  Do we have integrations to these tools already? 

**Adam:**

## This brings us to the final question that is, Can users contribute to the Keptn community since it is open source, If so, what are all things they can contribute?
**Adam:** 


V: You can always join the our community. To join please use the link below in the description which will take you to our slack workspace - Where future discussion of Keptn happens. 

 I really appreciate your time here, Adam. 

## What do you like to say to our listeners today? 
**Adam:** 

Thank you everyone for listening to the episode. We will bring you more so stay curious. For more information about Keptn, you can visit out site Kept.sh anytime. I am your host Vishruth Harithsa, signing off.

Adios and have a great time. 
