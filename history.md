# Cloud Control

## History

### v.1

I started this project as an answer for a small question: 
"What if I want to run EC2 instance using Alexa?"

And the first attempt was just like that. Create instance, 
check number of existing instances in specific state and terminate.

And it was cool :)

Then, I started to think, how to build something what will be 
at least usable.

### v.2

And that is how the second version was born. In this version, 
I started to implement (by learning, as I am not a programmer) 
more complicated logic. And I failed. 

I realized very fast, that what I want to achieve is more complex, 
than I expected.

### v.2.5

So, to go back on track, I started to design the dialogs. That was 
the main problem for me. Exemples available become simple very fast.

How to build the logic for intents, how to build the logic of each 
intent, etc, it was hard to figure out.

At those days I had the opportunity to attend AWS Summit in Warsaw, 
and I discussed my concerns with Alexa team. That was awesome. They 
recommend me a book how to build interaction, and that was a good step 
forward.

Eventually, I draw everything what I had in mind, and start building.

And I built the monster. 10M of code. As a Lambda function. Come on...
OK, I was really thrilled, it was working. I was able to create, change, 
delete, tag, untag and check instances. 

But it was too much for one function already, and I had plans...

### v.3

At this point I started to do what most of companies are doing / thinking about. 
I started to split monolith to single functions.

And also, I created a full CI/CD for it using Travis, SonarCloud and my own 
pylint container.

That was refreshing lesson, as I was thinking a lot how to describe the 
pipeline.

### Interlude

Now, this is done. So, base for SEC conference is ready.

I have a lot of ideas, what to do next. First, I plan to add 'context 
understanding' for Cloud Control. This will be pretty cool, to create 
something 'more human' in conversation.

Also, the plan is to add possibility to build instance on predefined AMIs 
(not some default like now), add S3 management, and the most important - 
CloudWatch management.

### v.4

Heh. I decided to switch Terraform to CloudFormation. It looks more clean for me, 
when run through TravisCI.  
My goal is to focus on this project, as it is selected as the topic on some meetups / conferences.
