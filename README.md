# Presentation and Note

>Udacity
Data Streaming:
1) OPT:

2) SF Crime:
1./usr/bin/zookeeper-server-start config/zookeeper.properties
2./usr/bin/kafka-server-start config/server.properties
3.python kafka_server.py
4.kafka-console-consumer --bootstrap-server localhost:9092 --topic com.udacity.project.sfcrimes --from-beginning


>ML presentation

```
1. Intro:
AI is changing the way we work and live and this nontechnical presentation will teach you how to navigate the rise of AI. Whether you want to know what's behind the buzzwords or whether you want to perhaps use AI yourself either in a personal context or in a corporation, this course will teach you how. Today's talk will give you a realistic view of what AI really is. 

There is a lot of excitement but also a lot of unnecessary hype about AI. Almost all the progress we are seeing in the AI today is artificial narrow intelligence. These are AIs that do one thing such as a smart speaker or a self-driving car, etc. However, AI also refers to a second concept of AGI or artificial general intelligence. That is the goal to build AI. They can do anything a human can do or maybe even be superintelligence and do even more things than any human can. I'm seeing tons of progress in ANI, artificial narrow intelligence and almost no progress to what AGI or artificial general intelligence. Both of these are worthy goals and unfortunately the rapid progress in ANI which is incredibly valuable, that has caused people to conclude that there's a lot of progress in AI, which is true. But that has caused people to falsely think that there might be a lot of progress in AGI as well which is leading to some irrational fears about evil clever robots coming over to take over humanity anytime now. I think AGI is an exciting goal for researchers to work on, but it'll take most for technological breakthroughs before we get there and it may be decades or hundreds of years or even thousands of years away. Given how far away AGI is, I think there is no need to unduly worry about it.

In this talk, I will introdue what ANI can do and how to apply them to some problems. Later in this talk you'll also see some case studies of how ANI can be used to build really valuable applications such as smart speakers and self-driving cars. You may have heard of machine learning and the next video will teach you what is machine learning. You also learn what is data and what types of data are valuable but also what does the data are not valuable. You learn what it is that makes a company an AI company or an AI first company so that perhaps you can start thinking if there are ways to improve your company or other organizations ability to use AI and importantly, you also learned this week what machine learning can and cannot do. 

In our society, newspapers as well as research papers tend to talk only about the success stories of machine learning and AI and we hardly ever see any failure stories because they just aren't as interesting to report on. But for you to have a realistic view of what AI and what machine learning can or cannot do, I think is important that you see examples of both so that you can make more accurate judgements about what you may and maybe should not try to use these technologies for.

Finally, a lot of the recent rise of, machine learning has been driven through the rise of Deep Learning. Sometimes also called Neural Networks. You can also see an intuitive explanation of deep learning so that you will better understand what they can do particularly for a set of narrow ANI tasks. Now we have a sense of AI technologies and what they can and cannot do. Next we'll see how these AI technologies can be used to build valuable projects. We also need to know what we should do to make sure we select projects that are technically feasible as well as valuable to our business. After learning what it takes to build AI projects, in the third week you'll learn how to build AI in your company. In particular, if you want to take a few steps toward making your company good at AI, you see the AI transformation playbook and learn how to build AI teams and also built complex AI products. 
Now, one of the major technologies driving the recent rise of AI is Machine Learning. But what is Machine Learning? Let's take a look in the next video.

2. What is Machine Learning:

The rise of AI has been largely driven by one tool in AI called machine learning. The most commonly used type of machine learning is a type of AI that learns A to B, or input to output mappings. This is called supervised learning. Let's see some examples. If the input A is an email and the output B one is email spam or not, zero one. Then this is the core piece of AI used to build a spam filter. Or if the input is an audio clip, and the AI's job is to output the text transcript, then this is speech recognition. More examples, if you want to input English and have it output a different language, Chinese, Spanish, something else, then this is machine translation. 
I'll define these terms more precise in later video, so don't worry too much about what it means for now.
The most important idea in AI has been machine learning, has basically supervised learning, which means A to B, or input to output mappings. 

Or if you want to build a self-driving car, one of the key pieces of AI is in the AI that takes as input an image, and some information from their radar, or from other sensors, and output the position of other cars, so your self-driving car can avoid the other cars.

This set of AI called supervised learning, just learns input to output, or A to B mappings.
On one hand, input to output, A to B it seems quite limiting. But when you find a right application scenario, this can be incredibly valuable. Now, the idea of supervised learning has been around for many decades. But it's really taken off in the last few years.

AI has really taken off recently due to the rise of neural networks and deep learning. I'll define these terms more precise in later video, so don't worry too much about what it means for now. 

with neural networks and deep learning, what we saw was that, if you train a small neural network, then the performance looks like this, where as you feed them more data, performance keeps getting better for much longer. If you train a even slightly larger neural network, say medium-sized neural net, then the performance may look like that. If you train a very large neural network, then the performance just keeps on getting better and better. For applications like speech recognition, online advertising, building self-driving car, where having a high-performance, highly accurate, say speech recognition system is important, enable these AI systems get much better, and make speech recognition products much more acceptable to users, much more valuable to companies and to users.
Now, a few couple of implications of this figure. If you want the best possible levels of performance, then you need two things: One is, it really helps to have a lot of data. So that's why sometimes you hear about big data. Having more data almost always helps. The second thing is, you want to be able to train a very large neural network. So, the rise of fast computers, including Moore's law, but also the rise of specialized processors such as graphics processing units or GPUs, make many many other companies to be able to train large neural nets on a large enough amount of data in order to get very good performance and drive business value. The most important idea in AI has been machine learning, has basically supervised learning, which means A to B, or input to output mappings. What enables it to work really well is data.

We need to know what data we have and how to feed this data into AI system.

3. Data:
It's up to you to decide what is A and what is B, and how to choose these definitions of A and B to make it valuable for your business. But how do you get data? How do you acquire data? Well, one way to get data is manual labeling. For example, you might collect a set of pictures like these over here, and then you might either yourself or have someone else go through these pictures and label each of them. Another way to get a dataset is from observing user behaviors or other types of behaviors. So, for example, let's say you run a website that sells things online. So, an e-commerce or an electronic commerce website where you offer things to users at different prices, and you can just observe if they buy your product or not. So, just through the act of either buying or not buying your product, you may be able to collected a data set like this, where you can store the user ID, the time the user visited your website, the price you offer the product to the users as well as whether or not they purchased it. So, just by using your website, users can generate this data from you. The third and very common way of acquiring data is to download it from a website or to get it from a partner. Finally, if you're working with a partner, say you're working with a factory, then they may already have collected a big dataset, machines, and temperatures, and pressure into the machines fail not that they could give to you. once you've started collecting some data, go ahead and start showing it or feeding it to an AI team. Because often, the AI team can give feedback to your IT team on what types of data to collect and what types of IT infrastructure to keep on building. For example, maybe an AI team can look at your factory data and say, "Hey. You know what? If you can collect data from this big manufacturing machine, not just once every ten minutes, but instead once every one minute, then we could do a much better job building a preventative maintenance systems for you." So, there's often this interplay of this back and forth between IT and AI teams, and my advise is usually try to get feedback from AI earlier, because it can help you guide the development of your IT infrastructure. More data is usually better than less data, but I wouldn't take it for granted that just because you have many terabytes or gigabytes of data, that an AI team can actually make that valuable. 

4. Terminology:
You might have heard terminology from AI, such as machine learning or data science or neural networks or deep learning. What do these terms mean? The boundaries between these two terms, machine learning and data science are actually little bit buzzy, and these terms are not used consistently even in industry today.

machine learning is the field of study that gives computers the ability to learn without being explicitly programmed. This is a definition by Arthur Samuel many decades ago. Arthur Samuel was one of the pioneers of machine learning, who was famous for building a checkers playing program.
So, a machine learning project will often results in a piece of software that runs, that outputs B given A. In contrast, data science is the size of extracting knowledge and insights from data. So, the output of a data science project is often a slide deck, the PowerPoint presentation that summarizes conclusions for executives to take business actions or that summarizes conclusions for a product team to decide how to improve a website.
Let me give an example of machine learning versus data science in the online advertising industry. Today, to launch our platforms, all have a piece of AI that quickly tells them what's the ad you are most likely to click on. So, that's a machine learning system. This turns out to be incredibly lucrative AI system to inputs enrich about you and about the ad and outputs where you click on this or not. These systems are running 24-7. These are machine learning systems that drive our gravity for these companies, such as a piece of software that runs. In contrast, I have also done data science projects in the online advertising industry. If analyzing data tells you, for example, that the travel industry is not buying a lot of ads, but if you send more salespeople to sell ads to travel companies, you could convince them to use more advertising, then that would be an example of a data science project and the data science conclusion the results and the executives deciding to ask a sales team to spend more time reaching out to the travel industry. So, even in one company, you may have different machine learning and data science projects, both of which can be incredibly valuable. 

You have also heard of deep learning. So, what is deep learning? 
Let's say you want to predict housing prices, you want to price houses. So, you will have an input that tells you the size of the house, number of bedrooms, number of bathrooms and whether it's newly renovated. One of the most effective ways to price houses, given this input A would be to feed it to this thing here in order to have it output the price. This big thing in the middle is called a neural network, and sometimes we also called an artificial neural network. That's to distinguish it from the neural network that is in your brain. So, the human brain is made up of neurons. So, when we say artificial neural network, that's just to emphasize that this is not the biological brain, but this is a piece of software. What a neural network does, or an artificial neural network does is takes this input A, which is all of these four things, and then output B, which is the estimated price of the house. But all of human cognition is made up of neurons in your brain passing electrical impulses, passing little messages each other. When we draw a picture of an artificial neural network, there's a very loose analogy to the brain. These little circles are called artificial neurons, or just neurons for short. That also passes neurons to each other. This big artificial neural network is just a big mathematical equation that tells it given the inputs A, how do you compute the price B. In case it seems like there a lot of details here, don't worry about it. We'll talk more about these details later. But the key takeaways are that a neural network is a very effective technique for learning A to B or input-output mappings. Today, the terms neural network and deep learning are used almost interchangeably, they mean essentially the same thing.
Many decades ago, this type of software was called a neural network. But in recent years, we found that deep learning was just a much better sounding brand, and so that for better or worse is a term that's been taken off recently. So, what do neural networks or artificial neural networks have to do with the brain? It turns out almost nothing. Neural networks were originally inspired by the brain, but the details of how they work are almost completely unrelated to how biological brains work. So, I choose very courses today about making any analogies between artificial neural networks and the biological brain, even though there was some loose inspiration there. 

You might also hear in the media other buzzwords like unsupervised learning, reinforcement learning, graphical models, planning, knowledge graph, and so on. You don't need to know what all of these other terms mean, but these are just other tools to getting AI systems to make computers act intelligently.

But the most important tools that I hope you know about are machine learning and data science as well as deep learning and neural networks, which are a very powerful way to do machine learning, and sometimes data science. If we were to draw a Venn diagram showing how all these concepts put together, this is what it may look like. AI is this huge set of tools for making computers behave intelligently. Off AI, the biggest subset is prairie tools from machine learning, but AI does have other tools than machine learning, such as some of these buzzwords, are listed at the bottom. The part of machine learning that's most important these days is neural networks or deep learning, which is a very powerful set of tools for carrying out supervised learning or A to B mappings as well as some other things. But there are also other machine learning tools that are not just deep learning tools. So, how does data science fit into this picture? There is inconsistency in how the terminology is used. Some people will tell you data science is a subset of AI. Some people will tell you AI is a subset of data science. So, it depends on who you ask. But I would say that data science is maybe a cross-cutting subset of all of these tools that uses many tools from AI machine learning and deep learning, but has some other separate tools as well that solves a very set of important problems in driving business insights. I hope this gives you a sense of the most common and important terminology using AI, and you can start thinking about how these things might apply to your company.


What makes an AI company:

What machine learning can and cannot do:

How to choose an AI project:
Machine learning is an “iterative” process, meaning that an AI team often has to try many ideas before coming up with something that’s good enough, rather than have the first thing they try work.
Say you want to use Machine Learning to help your sales team with automatic lead sorting. I.e., Input A (a sales prospect) and output B (whether your sales team should prioritize them). The 3 steps of the workflow, in scrambled order, are:
(i) Deploy a trained model and get data back from users
(ii) Collect data with both A and B
(iii) Train a machine learning system to input A and output B

Say you want to build an AI system to help recruiters with automated resume screening. Which of these steps might be involved in “technical diligence” process?  (Select all that apply.)
Defining an engineering timeline
Making sure you can get enough data for this project
Ensuring that this is valuable for your business (e.g., estimating the project ROI)
Making sure that an AI system can meet the desired performance

Which of these statements about “business diligence” do you agree with?
Business diligence is the process of ensuring that the envisioned AI technology is feasible.
Business diligence is the process of ensuring that the AI technology, if it is built, is valuable for your business.

Say you want to build an AI system to help recruiters with automated resume screening. Which of these steps might be involved in “technical diligence” process?  (Select all that apply.)
Defining an engineering timeline
Making sure you can get enough data for this project
Making sure that an AI system can meet the desired performance

Ensuring that this is valuable for your business (e.g., estimating the project ROI)

week2

Pitfall:
Before wrapping up this video one pitfall I want to urge you to avoid is expecting a 100% accuracy from your AI software. Here's what I mean, let's say this is your test set which you've already seen on the last slide. But, let me add a few more examples to this test set. Here are some of the reasons it may not be possible for a piece of AI software to be a 100% accurate. First, machine learning technology today despite being very powerful still has limitations and they just can't do everything. So, you may be working on a problem that it's just very difficult even for today's machine learning technology. Second, insufficient data. If you don't have enough data specifically if you don't have enough training data for the AI software to learn from it may be very difficult to get a very high level of accuracy. Third, data is messy and sometimes data can be mislabeled. For example, this green coffee mug here looks perfectly okay to me, so, the label of it being a defect looks like an incorrect label and that would hurt the performance of your AI software. Data can also be ambiguous.

AI technical tools:
Finally, you might hear about Cloud versus On-premises, or for short, On-prem deployments. Cloud deployments refer to if you rent compute servers such as from Amazon's AWS, or Microsoft's Azure, or Google's GCP in order to use someone else's service to do your computation. Whereas, an On-prem deployment means buying your own compute servers and running the service locally in your own company. A detailed exploration of the pros and cons of these two options is beyond the scope of this video. A lot of the world is moving to Cloud deployments. Whether you search online you find many articles talking about the pros and cons of Cloud versus On-prem deployments. 

Building AI in your company:
week3

As you can tell both from this rather complex example of an AI pipeline, as well as the early example of the four-step AI pipeline for the smart speaker, sometimes it takes a team to build all of these different components of a complex AI product. What I'd like to do in the next video is share with you what are the key roles in large AI teams. If you're either a one-person or small AI team now, that's okay, but I want you to have a vision of what building a large AI team, maybe in the distant future, might look like.

 I hope this survey of AI application areas gives you a sense that the wide range of data that AI is successfully applied to today, and maybe this even inspire you to think of how some of these application areas may be useful for your own projects. Now, so far the one AI technique we've spent the most time talking about is supervised learning. That means learning inputs, output, or A to B mappings from labeled data where you give the AI system both A and B. But that's not the only AI technique out there. In fact, the term supervised learning almost invites the question of what is unsupervised learning, or you might also have heard from media articles, from the news about reinforcement learning. So, what are all these other techniques? In the next video, the final optional video for this week, we'll do a survey of AI techniques, and I hope that through that maybe you'll see if some of these other AI techniques and supervised learning could be useful for your projects as well. Let's go on to the final optional video for the week.

 There are a lot of AI and machine learning techniques today. And while supervised learning, that is learning A to B mappings, is the most valuable one, at least economically today, there are many other techniques that are worth knowing about. Let's take a look. The best known example of unsupervised learning is clustering, here's an example. Let's say you run a grocery store that specializes in selling potato chips.

 For example, if you're trying to use supervise learning to get the AI system to recognized coffee mugs, then you may give it 1000 pictures of coffee mug, or 10,000 pictures of mug coffee mug. And that's just a lot of picture of coffee mugs coffee mug we will be giving our AI systems. For those of you that are parents, I can almost guarantee to you that no parent on this planet, no matter how loving and caring, has ever pointed out 10,000 unique coffee mugs to their children, to try to teach the children what is a coffee mug. So, AI systems today require much more labeled data to learn than when a human child or than would most animals. Which is why AI researchers hold a lot of hope out for unsupervised learning as way, maybe in the future, for AI to learn much more effectively in a more human like way, and more biological like way for much less labeled data.

 Why is developing an AI strategy NOT the first step in the AI Transformation Playbook?
Without having some practical AI experience and knowing what it feels like to build an AI project, a company usually does not know enough to formulate a sound strategy.

week4
limitations:
In fact, there's a lot it cannot do but it will transform industries and society. When you speak with friends about AI, I hope you also tell them about this Goldilocks rule for AI, so, that they too can have a more realistic view of AI. There are many limitations of AI. You have already seen earlier some of the performance limitations. For example, given a small amount of data, a pure AI probably cannot fully automate a call center and give very flexible responses to whatever customers are emailing you with. But AI has other limitations, as well. One of the limitations of AI is that explainability is hard and many high-performing AI systems are black boxes. Meaning that it works very well but the AI doesn't know how to explain why it does what it does.
Now, to be fair, humans are also not very good at explaining how we make decisions ourselves. For example, you've already seen this coffee mug in the last weeks videos but how do you know it's a coffee mug? How does a human look at this and say, that's a coffee mug? You know there are some things you can point to like, there's a room for liquid and it has a handle. But we humans are not very good at explaining, how we can look at this and decide what it is. But because AI is a relatively new thing, the lack of explainability is sometimes a barrier to its acceptance. Also, sometimes if an AI system isn't working then its ability to explain itself would also help us figure out how to go in and make the AI system work better. So, explainability is one of the major open research areas. A lot of researchers are working on. What I see in practice, is that when an AI team wants to deploy something, that AI team must often able to come up with an explanation that is good enough to enable the system to work and be deployed. So, explainability is hotbed, its often not impossible but we do need much better tools to help the AI systems explain themselves.

One question now sometimes asked is what should you do if you want to work in AI? Recently, a radiologist resident served radiologists near the start of his career. He actually asked me. He said, "Hey, Andrew, I'm hearing a lot about the coming impacts of AI on radiology." He said, "Should I quit my profession and just learn AI and do AI instead?" My answer to him was no. You could do that. You can actually quit whatever you are doing and pick up AI from scratch. It is entirely possible to do that. Many people have done that. This one other alternative that you could consider though, which is, I said to this radiology resident consider doing work in AI plus radiology because with your knowledge of radiology, if in addition you learned something about AI, you would be better positioned to do work at the intersection of radiology and AI than most other people. So, if you want to do more work in AI, it is possible in today's world to learn AI from scratch through online courses and other resources. But if you take whatever you are already knowledgeable in and learn some AI and do your area plus AI, then you might be more uniquely qualified to do very valuable work by applying AI to whatever area you are already an expert in. So, I hope this video helps you navigate the coming impacts of AI in jobs. Let's go on to the next and final video of this course.

Congratulations on coming to the last video of this course. AI is a super power, and understanding it allows you to do things that very few people on the planet can. Let's summarize what you've seen in this course. In the first week, you learned about AI technology, what is AI and what is machine learning? What's supervised learning, that is learning inputs, outputs, or A to B mappings. As well as what is data signs, and how data feeds into all of these technologies? Importantly, you also saw examples of what AI can and cannot do. In the second week, you learned what it feels like to build an AI project. You saw the workflow of machine learning projects, of collecting data, building a system and deploying it, as well as the workflow of data science projects. And you also learned about carrying out technical diligence to make sure a project is feasible, together with business diligence to make sure that the project is valuable, before you commit to taking on a specific AI project. In the third week, you learned how such AI projects could fit in the context of your company. You saw examples of complex AI products, such as a smart speaker, a self-driving car, the roles and responsibilities of large AI teams. And you also saw the AI transmission playbook, the five step playbook for helping a company become a great AI company. I hope these materials throughout these first three weeks can help you brainstorm AI projects or think about how you might want to use AI in your company or in your organization. In this week, week four, you learned about AI and society. You saw some of the limitations of AI beyond just technical limitations, and also learned about how AI is affecting developing economies and jobs worldwide. You've learned a lot in these four weeks, but AI is a complex topic. So I hope you will keep on learning, whether through additional online courses, through Coursera or deeplearning.ai, or books, or blogs, or just by talking to friends. If you ever want to try your hand at building AI technology, it is now easier than ever to learn to code and learn how to implement AI technology through these resources. If you'd like to keep on receiving information about AI, you can also sign up for the deeplearning.ai mailing list, by going to the deeplearning.ai website and signing up there. I'll occasionally send you useful information about AI through that mailing list.
Start transcript at 2 minutes 51 seconds2:51
Congratulations on finishing this course. You're now significantly ahead of many large companies' CEOs in your understanding of AI and your ability to plan for the rise of AI. So I hope that you provide leadership to others as well that are trying to navigate these issues. Lastly, I want to say to you, thank you very much for taking this course. I know that you're busy with your own work or school, and friends and family, and I'm grateful that you spend so much time with me and in this course learning these complex issues relating to both the technology and the impact of AI. So thank you very much for both the time and the effort you put Into this course.

```

http://solutionoptimist.com/2013/12/28/awesome-github-tricks/
