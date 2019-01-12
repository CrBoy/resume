# Pi, Yu-Chuan (CrBoy)
#Web #後端 #Ruby-on-Rails #JavaScript #DevOps #AWS #網管 #Linux

Contact: crazyscorpio@gmail.com

## Work Experiences
* CTO, Sharelike _2014 - 2018_
Backend development (CodeIgniter, Laravel, Rails); Frontend development (AngularJS, Vue.js); Administration of servers and cloud services (VMWare ESXi, Linode, AWS, G Suite); Administration of network devices
* Organizer, COSCUP (Conference of Open Source Coders, Users and Promoters) _2015 - 2017_
* Web Programmer, Computer Center of NCKU _2013 - 2014_
Web project development (PHP + customized CodeIgniter）
* Web Programmer, Computer Center of NCKU _2012 - 2012_
Course system, introducing Git, and technical sharing

## Education
* Master of Computer Science, National Cheng-Kung University (NCKU) _2009 - 2012_
* BS, Computer Science, National Cheng-Kung University (NCKU) _2005 - 2009_

## Technical Experiences
### Software Development
* Experience with several programming languages, such as PHP (5.x), Python (3.x), Ruby (2.2~), JavaScript (ES5 ~ ES6).
* Contributed more than 90% code of the long live product of Sharelike, using Ruby on Rails, MySQL and Redis.
* Made an admin dashboard for our FAE, using AngularJS and Bootstrap 3.
* Use Node.js making tools, which is frequently used includes:
	* Forward AWS CloudWatch Alarm to Slack.
	* An internal service as an SMS gateway, which sends the messages from staging environment to Slack and Telegram, to save money.
* Use Bash script, Python or Ruby making my own tools, e.g. updating website automatically, notifying me while tickets are available, or buying something popular. I also rewrite those tools in Node.js. With the feature of event-driven, I can burst mass requests, which is very nice for timing-sensitive operations.
* Attended Google Code Jam with Python in 2014. Passed into top 3000, but not top 500.
* Created [NCKU CSIE Wiki](http://wiki.csie.ncku.edu.tw/). I was not modifying the server-side of Gitit wiki system, but using the template, along with jQuery and Bootstrap, to make it much more pretty.
### Infrastructure Operation
* Built system of auto testing and deployment, which is applied to our frontend (Vue.js and Webpack) and backend (Rails and Sinatra) projects, with GitLab. There is also operational tasks running on CI, made simplifier.
* Administrating AWS accounts
	* Being the only AWS admin at Sharelike.
	* Using EC2, RDS, S3, CloudFront, etc. Making load balance by ELB as well, to increase API throughput, and prevent downtime.
	* Setup ECS cluster (nevertheless, with only ONE instance mostly) to run internal services, e.g. GitLab, and newly developing products, on which the staging and production run.
	* Using SES as SMTP service.
	* Creating lightweight services on API Gateway and Lambda, with no cost.
	* Applying SSL on most services, which is using the free certificates signed by AWS Certificate Manager. Some services use certs signed by Let's Encrypt.
	* To decrease human-interference on the infrastructure and achieve "infrastructure as code", we use CloudFormation to provision AWS resources. I wrote every template from scratch, not used CloudFormer to create it.
* Built and administrating networking infrastructure in Sharelike. I did the cabling, setup wired and wireless network, and split internal and external network by VLAN. I setup our own IP-PBX as well.
* I was the leader of info team in COSCUP 2018. I had coordinated and been doing the website development. We also make it auto build and deploy using GitHub Pages and Travis CI.
### Technical Sharing
* Gave talks with the topic "那些老師沒教的事 - Code Smart, Don't Code Hard" in 2012, which is about Git version control, gcc, make and gdb.
* Made technical sharing in my team. The topics include Git, Git flow, design pattern (Java), how-certificate-authority-works, and AWS, etc.
* Summarize my thoughts on web technology in 2015: [HTTP 通訊簡介](http://blog.crboy.net/2015/08/http.html). (No English version here)
### Miscellaneous
* Analyzing network using tcpdump, Wireshark and BurpSuite. I did this for understand the data flow of mobile apps which doesn't encrypt flow or implying certificate pinning. I also debugged my SIP service by network analysis.
* Found and [reported](https://zeroday.hitcon.org/vulnerability/ZD-2017-01260) a flaw of "17 Live" app with friends. The flaw is significant that is able to affect business.
* Found and [reported](https://zeroday.hitcon.org/vulnerability/ZD-2016-00074) a flaw of a KTV system. We gave a lightning talk about that on HITCON after reported.
* Familiar with command line, and able to touch-type.
