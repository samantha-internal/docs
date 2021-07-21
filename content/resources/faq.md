# FAQ

## Could you please explain your technology to a layman?

Whitehead is a simple and elegant API for common natural language tasks. You can use them to build games, chatbots, and novel conversational interfaces.

In non-technical terms, an API is a service that an app can “subcontract” certain tasks to. For instance, Uber uses the Google maps “API” for routing and in our case, you can use it for AI products that understand natural language.

## Could you explain natural language AI to a layman?

Natural language or plain English, French, Hindi etc, comes naturally to us and we use it to express all kinds of ideas to each other \(including this passage\). While being nearly effortless for humans, its nuances and countless associations with our surroundings make understanding natural language extraordinarily challenging using computer programs.

In the near future, voice will become an important mode of human-computer interaction at par with the visual and tactile UIs \(cellphones, laptops, etc.\) of today. Billions of experiences are going to use voice, both standalone and in conjunction with other modes of interactions. For this to happen, we are going to need tools and infrastructure that can capture and handle the nuances of human speech.

## What is context-aware AI?

Humans heavily rely on context or background information to understand meaning in discourse and conversations. For example, “Why did John not iron the shirt inside-out?” makes sense only given that one knows what a shirt is and what “iron”ing it entails but also that “iron” here is not the name of a metal and that shirts have an “inside”.

Understanding context is the biggest challenge for programs to understand human language. We offer one of the first APIs in the space that can adapt its output on the basis of information from the “context” provided by the application.

For example, our _smartcomplete_ API can complete a sentence intelligently taking background info in account, like so: `smartcomplete(“Hey John, I am not available today but can we schedule a call for…”, “Today is Monday”)` would return something like `“Tuesday or Wednesday?”`

Similarly, our chitchat service bases its next response on the history of the conversation, and so on.

## Do you license your SDKs?

No, we don't use a license-based pricing model. All of our SDKs are simply there to call our APIs from your own code. Our SDKs are based on an open-source, non-commercial license.

## Is Whitehead a framework?

No, we are an on-demand api service.

## Is Whitehead for beginners or non-experts only?

No, it is an API platform that provides access to state-of-the-art natural language understanding tools. we keep the models up-to-date, train them, manage GPUs and run inference while you focus on building awesome NL/conversational apps.

Analogy: You could always build your own navigation system but depending on your use case, it might be better to use google maps API.

## Is Whitehead AI right for me?

This is the classic build-vs-buy question. If our feature sets solve problems for your app/use case then the answer is: it depends. This topic has been well discussed in the industry and you can read more [here](https://www.forbes.com/sites/forbestechcouncil/2020/03/04/build-vs-buy-why-most-businesses-should-buy-their-next-software-solution/?sh=3e3601311280) and [here](https://medium.com/adobetech/when-to-build-vs-buy-enterprise-platform-risks-benefits-and-considerations-fea358449b30).

Excerpt from [the Forbes article](https://www.forbes.com/sites/forbestechcouncil/2020/03/04/build-vs-buy-why-most-businesses-should-buy-their-next-software-solution/?sh=3e3601311280) **Build Vs. Buy: Why Most Businesses Should Buy Their Next Software Solution**:

> The burden of product development, quality assurance, maintenance, platform migration and patch fixes are owned by the solution provider, while in-house development will usually require years of continued development beyond the initial project scope. In most cases, the vendor gains efficiencies because of its large customer base, so it can often charge less for implementing and maintaining an established product than it would cost to support a one-off, homegrown application.

> Plus, as a customer of a commercially available solution, your key users will have input to new features released on a regular basis -- developed in extensive collaboration with your provider’s user base.

## Do you allow training custom models?

Yes, this feature is not yet generally available but soon, you will be able to train \(or more accurately finetune\) nearly all of our APIs.

## How is this different from Rasa?

[Rasa](https://rasa.ai) is a Python framework for building chatbots, it is free and open-source but you need to train and host your own models and do the legwork required for building the dialog engine. Using Rasa gives you a lot of low-level control but you need to put in regular effort to keep your models up to date.

On the other hand, Whitehead is an API service providing NL tools on-demand. Nearly all of our models are zero-shot \(meaning they are ready to use off-the-shelf without any training/finetuning required\) and include a wide gamut of natural language tasks not limited to just conversational AI or chatbots but also other common non-dialog NLU tasks like paraphrasing, semantic search, etc.

## What is the future of AI in voice/conversation technology?

If you look at the evolution of human-computer interfaces over the years, it becomes apparent that we have been slowly extending our “senses” and “actuators” via technology and computing devices. We can see using “VR”, read, write, move around. And while we could “talk” to one another over computing media \(phones, VoIP\) for some time now, we have only had limited ability to talk “to” the computers themselves. This is changing with the advent of machine learning but we have just begun. Just like how our “tactile” devices matured from the first browsers and desktops to iPhones etc, better nlp tools will usher in computer programs that you can talk to as fluently as you would to a neighbor. I think that would be very interesting.

## How are you ensuring that your technology is inclusive and eliminates bias in the data sets and overall AI?

This is a very difficult problem and we are taking measures to tackle it.

First and foremost, bias thrives in biased environments. We aspire to be an international team with a healthy representation of cultures and identities.

Second, a lot of care has been taken in choosing our datasets to minimize discriminatory inputs. However, this can only go so far since these are too big for manual sieving and so we participate in OpenAI’s ethics initiative to disclose our modes of data selection so that our consumers can make better choices and take appropriate measures.

