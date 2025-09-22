---
title: The Health Debt of Sitting All Day (and How to Pay It Off)
date: 2025-09-22 19:00:00 +0100
categories: [Lifestyle, Development]
tags: [Health, Fitness, Software Development, Habits, Heart Health]
description: It is easy to put health at the back of our minds, especially when we feel fine with our current routines and lifestyles. But what happens to our bodies when we spend most of our careers sitting? 
---

# The Health Debt of Sitting All Day (and How to Pay It Off)

According to the World Health Organization, Heart Disease is one of the top causes of death: “[The WHO’s top 10 causes of death](https://www.who.int/news-room/fact-sheets/detail/the-top-10-causes-of-death)”. Along with that the WHO has consistent messaging that Cardiovascular diseases are preventable through changes in lifestyle habits [The WHO’s cvds fact sheet](https://www.who.int/news-room/fact-sheets/detail/cardiovascular-diseases-(cvds)). 

In this blog post I aim to explore the effects of spending hours on end in a chair has on our cardiovascular health and how we can work to prevent heart health problems with some simple lifestyle changes. As developers, we debug our code daily. I suggest we take that analytical nature we have and turn it in on ourselves, edit our default config to better optimize for heart health and longevity. 

## The Sitting Bug 

You might not be fully convinced of the fact that sitting can really impact our health in a meaningful way, and I don’t blame you! It’s just something that we all do as part of a normal day after all, what's the big deal? 

As crazy as it might seem there are actually multiple surprising effects that prolonged sitting across a career can have on our health, which we would probably rather avoid. Here are a few that I have come across in my research for this blog post: 

### Metabolic slowdown 

When we sit for a prolonged period we, obviously, use less energy/calories than we would otherwise. This, across the decades, can lead to possible weight gain, metabolic issues and eventually it could even contribute towards Diabetes. This is because a lack of physical activity affects the body’s ability to properly regulate blood sugar and blood pressure which could explain the link between sitting and metabolic slowdown, eventually leading to Type 2 Diabetes. Here are some links for further reading from [The NHS](https://www.nhs.uk/live-well/exercise/exercise-guidelines/why-sitting-too-much-is-bad-for-us/) and [The Mayo Clinic](https://www.mayoclinic.org/healthy-lifestyle/adult-health/expert-answers/sitting/faq-20058005). 

### Blood Clots 

It doesn’t end with metabolic issues, sitting brings us issues with blood flow and can contribute to the risks of blood clots! (Something we deffo want to avoid!) This one sounds particularly scary to me. This occurs when blood clots form in veins deep in our bodies (often our legs, where blood can pool and stagnate when sitting) and when left untreated can transform into a life-threatening condition where a clot can break free from its original position and travel to the lungs, leading to a [pulmonary embolism](https://www.nhs.uk/conditions/pulmonary-embolism/). This is the reason behind the suggestion to wear compression socks on long distance flights. Luckily, this is preventable with movement! For further reading on blood clots and sitting I suggest having a peruse of [this article](https://www.ahchealthenews.com/2025/03/25/prolonged-sitting-risk-for-dvt/) from advocate health care. 

### Cardiovascular Disease 

This is basically any disease related to the cardiovascular system such as stiff arteries, blockages, heart disease and heart attacks, etc. The mechanism behind how our risk goes up with prolonged sitting is similar to what was covered in the “Blood Clots” section above. There is a long list of reasons behind why low physical activity puts at high risk such as Endothelial Dysfunction, Chronic low-grade Inflammation, Insulin Resistance, etc. But the good news is that most of them have the same fix! ... **Move More**, it really does seem to be that simple. 

If you are interested in learning more here are some good sources for further reading: 

- [Short-Term Physical Inactivity Induces Endothelial Dysfunction](https://www.frontiersin.org/journals/physiology/articles/10.3389/fphys.2021.659834/full) 
- [Prolonged sitting and peripheral vascular function: potential mechanisms and methodological considerations](https://pubmed.ncbi.nlm.nih.gov/36794688/) 
- [Sedentary time in adults and the association with diabetes, cardiovascular disease and death](https://pubmed.ncbi.nlm.nih.gov/22890825/) 

Every prolonged period of sitting is adding onto our health debt, if we don’t make regular deposits to pay it off our health debt will continue to grow. 

## Improving Heart Health 

Did you know that our hearts beat an average of 100,000 per day? That’s about 36 million reps our hearts put in every year to keep us going. Our hearts are constantly putting in the work for us, trying its best through whatever we throw at it. Our hearts are so determined that they can even continue to beat after they are removed from our bodies?! So it seems only fair that we start to put in some effort to allow our hearts to keep doing what they love doing the most, pumping! 

There are many different risk factors around cardiovascular health, some are modifiable and within our control, but some are just the constants that will be with us through our run time. Let’s delve into the yaml file of our lifestyles to see what settings we can tweak to improve performance: 

```yaml
heartServer: 
  config: 
    # Some parameters are hardcoded by 'manufacturer' (non-modifiable) 
    non_modifiable: 
      Age:  
        value: "auto" 
        locked: true 
      Sex: "value=auto; locked=true" 
      Genetics: 
        value: "inherited" 
        locked: true 
      Ethnicity:  
        value: "inherited" 
        locked: true 
 
    # These settings are runtime configurable (modifiable risk factors) 
    modifiable: 
      Weight: 
        target: "healthy_BMI" 
        action: "optimize_diet, increase_activity" 
      CoMorbidities: 
        monitor: true 
        action: "medical_management" 
      Smoking: 
        enabled: false 
      Alcohol: 
        limit: "moderation" 
        warning: "cardio_toxic" 
      DrugUse: 
        enabled: false 
      PhysicalActivity: 
        steps_per_day: 10000 
      Diet: 
        quality: "balanced" 
        guidelines:  
          - "reduce processed foods" 
          - "increase fiber intake" 
          - "prefer healthy fats" 
``` 

The most significant risk factors, congenital heart defects aside, we are in control of. We can control if we smoke, what we eat and if we move. The World Health Organization has put out consistent messaging that most premature cardiovascular issues are preventable. This puts health back into our hands. Even if you have some genetic risk factors for cardiovascular issues, you can still prevent them from manifesting by making modifications to your day-to-day habits, even small changes can have a big impact over a lifetime. Remember, “It might be genetics that loads the gun, but its lifestyle that pulls the trigger” - Dr. Michael Greger. 

## Quick Wins: Small, Consistent Optimizations 

The main take away I want readers to have is to break up their sitting sessions and to get moving. Get some more steps to your routine, stretch out more often, stand up whenever you get a chance. Small but consistent changes can be a real-life saver! 

When I first started ___to want___ to make the conscious effort to get up and move I was rubbish at it, I would always forget! So, I went digging through my boxes to find my dusty sports watch because that has notifications to remind you to move... I would simply ignore the alerts or think "I will in a sec, let me finish writing this method then I'll get up" but always just forget afterwards. I have finally found something that works for me! As strange as this sounds, I keep a big cup of water on my desk and drink it as I'm coding, this makes me go to the toilet far more often and therefore I always remember to get up and move throughout the day. While I’m already up I do a few stretches, shake off my limbs, maybe do a couple of little squats and I'm back to it. It's been working great. And every time the cup is empty is another reason to get up to fill it up. This sounds daft but it works for me. Experiment and find something that works for you, perhaps the watch movement alerts will work for you, or a desktop movement timer/alert. The important thing is to break up your long periods of sitting as often as practical. 

### Get a few extra steps in 

The best way to get more movement in our daily routines, reduce our risk factors for cardiovascular diseases and metabolic slowdown is to simply get more steps in every day. It’s one of the most accessible forms of physical activity yet is often overlooked when people look to get fit. Adding just a few hundred extra steps into your routine can unlock significant benefits for both your physical and mental wellbeing. 

One magic number you might have heard before is to target 10,000 steps per day. That’s the goal I like to have because it’s a nice round number and is often recommended as a step count goal. However, the 10,000 goal never actually came out of any real scientific recommendation. It originated from a Japanese marketing campaign for a pedometer from the 1960s. Walking 10,000 steps per day is undoubtedly beneficial, more recent science suggests that health benefit gains flatten off at around 8,500 steps per day. 

One of the most effective tools in helping people include more movement in their life via steps is a simple step counter/pedometer or a fitness tracker (think Apple Watch or Garmin). A [study published in JAMA](https://jamanetwork.com/journals/jama/article-abstract/209526#25355299) has demonstrated that individuals who use a pedometer significantly increase their daily steps when compared to those who don’t use a pedometer. The research showed that using an activity tracker led to an average increase of about 2,100 steps per day over baseline, highlighting their influence on behavioral change. It also suggested the use of a pedometer, from the increased activity, was associated with significant decreases in body mass index and blood pressure. So, even if you don’t care to count your daily steps, I recommend investing in some kind of pedometer as it just might motivate you to get moving. 

There are many other ways to squeeze more steps into your busy lifestyle beyond just purchasing a smart watch. One of my favorite recent additions is getting into the automatic habit of a post-lunch stroll. I’ve been doing this for the past month and now as soon as I take the last bite of my lunch my brain goes straight “okay then, time to go for a walk”! With the weather getting colder, time will tell if this will stick. Even just a quick 10-15 min walk can make a big difference. And why not drag your pair-programmer along with you for some company and remind them the importance of movement; it’s a great way to clear your head after a busy morning. Perhaps your packed calendar just doesn't allow for you to consistently get a walk in every day? Then you can consider becoming an opportunistic walker, whenever greeted with an elevator simply take the stairs, pace around during phone calls or walk to and from work if it's feasible. Another way I’ve managed to sneak in some more movement is to stand or pace while waiting for the test suite to complete or during a project build. 

One of the main points of this article is prolonged sitting might be harmful to health and movement might be the saving grace. So, what about standing desks? Then we won’t be sitting all day! Standing desks are a really good way to break up sedentary time and if you are in a position where one is available to you then definitely make use of it. However, if like me, you don’t have access to a standing desk then don’t stress because the primary objective here is to move more frequently and consistently throughout a given day. Static standing is better than static sitting, but movement is what lowers our risks of cardiovascular health issues. 

## Closing  

Improving your heart health and increasing your step count doesn’t demand radical changes. Remember to keep it small and don’t over engineer it – KISS (Keep It Simple Stupid). Just pick a couple of small habits that are already easy to add to your current routine and make a conscious effort to keep those habits going, then once those are your new norm keep building from there. 

Cardiovascular disease is a progressive disease, so it is never too late and especially never too early to get started improving your health. Just get started, however small. Don’t fall into the trap of “I’ll get healthy when I’m older, for now I just need to enjoy life”. No one is asking you to give up the fun stuff. But the sooner you start, the better health outcomes we will see. 

Our hardware was not designed for the sedentary life we have found ourselves in. Just like if you are working on a PR and spot some messy legacy code, follow the boy scout rule and clean it up! Follow the boy scout rule and refactor your routine by adding one of the movement habits discussed in this blog post. 

Which habit are you going to add this week?
