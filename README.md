# EAAD-Group-D

* Applications of emotion recognition for maintaining the safety of an autonomous vehicle

## Procedure

![](https://i.imgur.com/VJkQOB5.png)

## Literature

* [Passengersâ€™ Emotions Recognition to Improve Social Acceptance of Autonomous Driving Vehicles](https://link-springer-com.eaccess.ub.tum.de/chapter/10.1007/978-981-15-5093-5_3)
* [Driver Emotion Recognition for Intelligent Vehicles: A Survey (June 2020)](https://dl-acm-org.eaccess.ub.tum.de/doi/pdf/10.1145/3388790)
  - Navigation voice as method to "control" emotion of driver / passengers (Mentioned here and refered to papers)
  - ![image](https://user-images.githubusercontent.com/66301041/116667380-6639fa00-a99c-11eb-92ba-6233556618c9.png) 
* [Happy-anger emotions classifications from electrocardiogram signal for automobile driving safety and awareness](https://www-sciencedirect-com.eaccess.ub.tum.de/science/article/abs/pii/S2214140516303693)
* [Advancements and recent trends in emotion recognition using facial image analysis and machine learning models](https://ieeexplore-ieee-org.eaccess.ub.tum.de/document/8284512)
* [Keep Calm and Ride Along: Passenger Comfort and Anxiety as Physiological Responses to Autonomous Driving Styles](https://dl.acm.org/doi/pdf/10.1145/3313831.3376247?casa_token=Qu_HFEDwdj4AAAAA:sLcxVV1rRLz17xA8zJol2VFWiRbDC8X-Ro-6XKE741kI1IcZfu7SRTxolI2hXbYqH6b1OvjtA5uvcg)
* [Emotional GaRage: A Workshop on InCar Emotion Recognition and Regulation ](https://dl.acm.org/doi/pdf/10.1145/3239092.3239098?casa_token=Cr0MnnNqjroAAAAA%3A3fdlKhy9jrnd6JAunrhFGIJQNncY0VrbvqhmhMiN97kkfrIcuLouLPelaqQacw7-sAdxurc50-857A)
  - links relatively new papers (2016-2018) for emotion detection
  - important in all levels of automation
    - Mauel driving: 
      - semi-autonomous driving: adjust timing of takeover depending on emotions
      - counteracts for frustration and agression: speech-based systems, play music or massagingfunction in the seat (emotion is detected)
      - Important for safety
    - Autonomous driving: 
      - confused (HMI design) or scared (driving style) driver
      - counteracts for frustration and agression: apply cognitive emotion regulation strategies, suggest relaxing movies/ music, display messages from friends, adapt smoother driving (emotion is detected)
      - Important for user acceptance
* [Automatic Emotion Recognition for the Calibration of Autonomous Driving Functions](https://www.mdpi.com/2079-9292/9/3/518)
* [Emotion recognition for semi-autonomous vehicles framework](https://link.springer.com/article/10.1007/s12008-018-0473-9)
* [Towards Multimodal Emotion Recognition in German Speech Events in Cars using Transfer Learning](https://arxiv.org/pdf/1909.02764.pdf)
* [Continuous Emotion Recognition via Deep Convolutional Autoencoder and Support Vector Regressor](https://arxiv.org/pdf/2001.11976.pdf)
* [Drive Safe: Cognitive-Behavioral Mining for Intelligent Transportation Cyber-Physical System](https://arxiv.org/pdf/2008.10148.pdf)

---
## 0510 Mei-Ju Part for Speech and CAN Behavior

* Sensing and Preprocessing

    - Speech

        - Voice Quality

            - Recording Setting

                - Type of Microphones
                - placement

            - Noise Reduction

                - amplify relevant acoustic signals
                - remove other overlapping noise

    - Behavior for driver

        - grip strength
        - gas and brake pedals with force sensors to capture leg motion
        - pressure sensors on the seat to track changes in body posture

* Analysis & Recongnition

    - Speech

        - Reduce the dimensionality for feature selection
        - Advanced Paper:

            - [Towards Multimodal Emotion Recognition in German Speech Events in Cars using Transfer Learning](https://arxiv.org/pdf/1909.02764.pdf)
            - Sep 2019
            - Goal: How to recognize driver's emotion by the audio signal of a spoken interaction, the visual signal of the driverâ€™s face, and the manually transcribed content of utterances of the driver. 
            - Method: Transfer learning + BiLSTM

    - Behavior

        - Relation between different behavioral changes and emotions

            - grip strength significantly varied for both anger and happiness 
            - measure stress by using the steering angle and a mass spring damper model 

        - Advanced Paper:
        
            - [Drive Safe: Cognitive-Behavioral Mining for Intelligent Transportation Cyber-Physical System](https://arxiv.org/pdf/2008.10148.pdf)
            - Aug 2020
            - Goal: Road Safety for Driver (focus on distraction detection)
            - Methods: capsule network, maximum likelihood, convolutional neural network, Apriori algorithm, and Bayesian network

---
## Comparaison

* [Google Excel for Paper Summary](https://docs.google.com/spreadsheets/d/18k6Jx_4VeK_lypwkIREGcaDZPzUHlqBQKtNft-X7Mfg/edit?usp=sharing)
* [Slides for Presentation](https://docs.google.com/presentation/d/19dKgfZl-CTtuMnRiy_aveLTkNYfGI-9jYAZ4pGj2Bi8/edit?usp=sharing)
* [Latex for Report](https://latex.tum.de/3146929735hfsbtvxmkppv)

---
## Discussion Notes

* 0423 Meeting

  - What **"Safety"** means ?
    
    - Teacher Answer
    - **Focus on in-cabin** environment. From the safety perspective there is no distinction between driver and passengers in in-cabin environment.
    - Consider two main directions of "full autonomy" and "partial autonomy" as the main story line of your research and try to define your research questions accordingly. In that case, you can properly distribute the applications by their target group (either on "driver-only" or "driver+passenger").
    - **Cover both directions (Driver + passengers) to discuss**
    - Your applications can be related to either comfort domain or driving dynamics, which the latter has the highest impact on safety. 

  - Read more literatures **at least ten**
  - need to complete comparison table

* 0430 Meeting

  - Follow this direction
  - ![image](https://user-images.githubusercontent.com/66301041/116667380-6639fa00-a99c-11eb-92ba-6233556618c9.png) 
  - JuliaďĽšFocus on **Camera** & **Biosensors**
  - Mei-Ju: Focus on **Microphones** & **CAN-Bus Steering Wheel Seat**
  - Next discussion, we need to organize the outline of the presentation 

* Fist Presentation/ Paper Structure Draft Julia:
	1. Intro: 
		- Importance of Emotional Awareness in all stages of automation (Manuel vs. Semi-automated vs. Fully Autonomous)
			- Differentiatle importance / impact / safety concerns
	2. Main Part: How to detect emotional awareness (Sensoring)
	3. What to do with the result of detected emotion? (Interpretation, Reaction of System on emotion)
		- Optional: close the cycle by adopting to the levels of automation (if not always mentioned besides)

* 0510 Discussion

**<Outline of Presentation>**

1. Introduction
* Define what is safety in our topic
* Emotional Awareness in all stages of automation (Manuel vs. Semi-automated vs. Fully Autonomous)
* Differentiatle importance / impact / safety concerns

2. Main
* Architecture
	- ![image](https://user-images.githubusercontent.com/66301041/116667380-6639fa00-a99c-11eb-92ba-6233556618c9.png)
* Separately talk about 4 Topics: Camera, Biosensors, Speech, CAN Behavior
	- How to detect emotional awareness (Sensoring & Preprocessing)
		- Challenges
	- Advanced Method (Analysis & Recognition)
	- What to do with the result of detected emotion for safety?
	- Importance: Emotional Awareness in all stages of automation

3. Comparison (pros and cons) of 4 Topics we mention for safety
4. Conclusion

* 0521 Discussion
	
	- Go through each part of our slides

* Next discussion on 05/25 (Tue) 16:00 , we would focus on slides **final** content and make sure its consistency


---
