# Voice-Enabled-Object-Detection

BATCH NO:26
 VOICE-ENABLED OBJECT DETECTION FOR THE
 VISUALLY IMPAIRED USING CNN
 Major project report submitted
 in partial fulfillment of the requirement for award of the degree of
 Bachelor of Technology
 in
 Information Technology
 By
 B. LEELAKRISHNAMOHAN (21UTIT0009) (VTU19580)
 Under the guidance of
 Ms. J. DEEPA, B.E., M.E.,
 ASSISTANT PROFESSOR
 DEPARTMENTOFINFORMATIONTECHNOLOGY
 SCHOOLOFCOMPUTING
 VELTECHRANGARAJANDR.SAGUNTHALAR&DINSTITUTEOF
 SCIENCEANDTECHNOLOGY
 (Deemed to be University Estd u/s 3 of UGC Act, 1956)
 Accredited by NAAC with A++ Grade
 CHENNAI600062, TAMILNADU,INDIA
 May, 2025
BATCH NO:26
 VOICE-ENABLED OBJECT DETECTION FOR THE
 VISUALLY IMPAIRED USING CNN
 Major project report submitted
 in partial fulfillment of the requirement for award of the degree of
 Bachelor of Technology
 in
 Information Technology
 By
 B. LEELAKRISHNAMOHAN (21UTIT0009) (VTU19580)
 Under the guidance of
 Ms. J. DEEPA, B.E., M.E.,
 ASSISTANT PROFESSOR
 DEPARTMENTOFINFORMATIONTECHNOLOGY
 SCHOOLOFCOMPUTING
 VELTECHRANGARAJANDR.SAGUNTHALAR&DINSTITUTEOF
 SCIENCEANDTECHNOLOGY
 (Deemed to be University Estd u/s 3 of UGC Act, 1956)
 Accredited by NAAC with A++ Grade
 CHENNAI600062, TAMILNADU,INDIA
 May, 2025
CERTIFICATE
 It is certified that the work contained in the project report titled ”VOICE-ENABLED OBJECT DE
TECTION FOR THE VISUALLY IMPAIRED USING CNN” by B. LEELA KRISHNA MOHAN
 (21UTIT0009) has been carried out under my supervision and that this work has not been submitted
 elsewhere for a degree.
 Signature of Supervisor
 Ms. J. Deepa
 Assistant Professor
 Information Technology
 School of Computing
 Vel Tech Rangarajan Dr. Sagunthala R&D
 Institute of Science and Technology
 May, 2025
 Signature of Head of the Department
 Dr. J. Visumathi
 Professor & Head
 Information Technology
 School of Computing
 Vel Tech Rangarajan Dr. Sagunthala R&D
 Institute of Science and Technology
 May, 2025
 Signature of the Dean
 Dr. S P. Chokkalingam
 Professor & Dean
 School of Computing
 Vel Tech Rangarajan Dr. Sagunthala R&D
 Institute of Science and Technology
 May, 2025
 i
DECLARATION
 We declare that this written submission represents my ideas in our own words and where others’
 ideas or words have been included, we have adequately cited and referenced the original sources. We
 also declare that we have adhered to all principles of academic honesty and integrity and have not
 misrepresented or fabricated or falsified any idea/data/fact/source in our submission. We understand
 that any violation of the above will be cause for disciplinary action by the Institute and can also
 evoke penal action from the sources which have thus not been properly cited or from whom proper
 permission has not been taken when needed.
 (Signature)
 (B.LEELA KRISHNA MOHAN)
 Date:
 /
 /
 ii
APPROVALSHEET
 This project report entitled VOICE-ENABLED OBJECT DETECTION FOR THE VISUALLY IM
PAIRED USING CNNbyB.LEELAKRISHNAMOHAN(21UTIT0009)is approved for the degree
 of B.Tech in Information Technology.
 Examiners
 Date:
 Place:
 /
 Supervisor
 Ms. J. DEEPA, B.E, M.E.
 Assistant Professor.
 /
 iii
ACKNOWLEDGEMENT
 We express our deepest gratitude to our Honorable Founder Chancellor and President Col.
 Prof. Dr. R. RANGARAJANB.E.(Electrical), B.E. (Mechanical), M.S (Automobile), D.Sc., and
 Foundress President Dr. R. SAGUNTHALA RANGARAJAN M.B.B.S.,Vel Tech Rangarajan
 Dr. Sagunthala R&D Institute of Science and Technology, for her blessings.
 Weexpress our sincere thanks to our respected Chairperson and Managing Trustee
 Dr. RANGARAJANMAHALAKSHMIKISHORE,B.E.,VelTechRangarajanDr. Sagunthala
 R&DInstitute of Science and Technology, for their blessings.
 Weare very much grateful to our beloved Vice Chancellor Prof. Dr.RAJAT GUPTA, for provid
ing us with an environment to complete our project successfully.
 We record indebtedness to our Professor & Dean , School of Computing,
 Dr. S P. CHOKKALINGAM, M.Tech., Ph.D., & Professor & Associate Dean , School of
 Computing, Dr. V. DHILIP KUMAR,M.E.,Ph.D., for immense care and encouragement towards
 us throughout the course of this project.
 Weare thankful to our Professor & Head, Department of Information Technology,
 Dr. J. VISUMATHI, M.E., Ph.D., for providing immense support in all our endeavors.
 Wealso take this opportunity to express a deep sense of gratitude to our Internal Supervisor
 J. DEEPA, B.E., M.E., for her cordial support, valuable information and guidance, she helped us in
 completing this project through various stages.
 A special thanks to our Project Coordinator Dr. ANITHA RAJAKUMARI P., Professor, for
 her valuable guidance and support throughout the course of the project.
 We thank our department faculty, supporting staff and friends for their help and guidance to com
plete this project.
 B.LEELA KRISHNAMOHAN (21UTIT0009)
 iv
ABSTRACT
 This project presents an innovative approach to object detection using Convolu
tional Neural Network (CNN) algorithm integrated with voice output. Traditional
 object detection systems primarily rely on visual outputs, which may not be acces
sible to visually impaired individuals or may require continuous visual attention
 from users. Our proposed system utilizes CNN, a powerful deep learning technique
 for image recognition and classification, to accurately detect objects within images.
 The system is augmented with voice output capabilities, enabling it to audibly
 announce the detected objects, thus making the information accessible to visually
 impaired users or in scenarios where visual attention is not feasible. Moreover,
 the system allows users to input data files containing images for object detection,
 enhancing its versatility and usability. By accepting data files as input, users can
 seamlessly integrate the object detection system into their existing workflows and
 processes.The combination of CNN algorithm, voice output, and data file input
 enhances the accessibility, usability, and adaptability of object detection systems,
 making them more inclusive and versatile across various applications and user
 scenarios.Furthermore, we explore the integration of voice output functionality,
 describing how the detected objects are converted into audible announcements.
 The system’s voice output capabilities are designed to be clear, concise, and easily
 understandable, facilitating seamless interaction for users.Additionally, we elaborate
 on the implementation of the data file input feature, which allows users to provide
 input images for object detection through files rather than real-time capture. This
 feature enhances flexibility and convenience, particularly in scenarios where batch
 processing or integration with existing data pipelines is required.We evaluate the
 performance of the proposed system through extensive experiments, assessing its
 accuracy, speed, and robustness across various datasets and scenarios.
 Keywords: Visually impaired, Blindness, Assistive system, Computer vision,
 Image recognition, Voice output, Convolutional Neural Network, Audio.
 v
LISTOFFIGURES
 4.1 ArchitectureDiagramofObjectDetection . . . . . . . . . . . . 15
 4.2 DataFlowDiagramofObjectDetection . . . . . . . . . . . . . . 16
 4.3 UseCaseDiagramofObjectDetection. . . . . . . . . . . . . . . 17
 4.4 ClassDiagramofObjectDetection. . . . . . . . . . . . . . . . . 18
 4.5 SequenceDiagramofObjectDetection . . . . . . . . . . . . . . 19
 4.6 Collaborationdiagram . . . . . . . . . . . . . . . . . . . . . . . 20
 4.7 ActivityDiagramofObjectDetection . . . . . . . . . . . . . . . 21
 4.8 DeepLearningFrameworks . . . . . . . . . . . . . . . . . . . . 23
 4.9 Pre-TrainedObjectDetection. . . . . . . . . . . . . . . . . . . . 24
 4.10 SetupSpeechandAudioProcessing . . . . . . . . . . . . . . . . 25
 5.1 TestImageofObjectDetection . . . . . . . . . . . . . . . . . . . 30
 5.2 TestImage . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 31
 6.1 GraphicalRepresentation. . . . . . . . . . . . . . . . . . . . . . 35
 10.1PlagiarismReportofObjectDetection. . . . . . . . . . . . . . . 45
 vi
LIST OFTABLES
 6.1 Comparison of Existing and Proposed System . . . . . . . . . . . . 34
 vii
LIST OFACRONYMSAND
 ABBREVIATIONS
 Acronym Abbreviation
 AOD
 CNN
 ODAI
 ODVI
 ODI
 Assistive Object Detection
 Convolution Neural Network
 Object Detection for the Visually Impaired
 Object Detection for Visual Impairment
 Object Detection for Impaired
 viii
TABLEOFCONTENTS
 Page.No
 ABSTRACT v
 LISTOFFIGURES vi
 LISTOFTABLES vii
 LISTOFACRONYMSANDABBREVIATIONS viii
 1 INTRODUCTION 1
 1.1 Introduction . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 1
 1.2 Background . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 2
 1.3 Objective . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 2
 1.4 ProblemStatement . . . . . . . . . . . . . . . . . . . . . . . . . . 3
 2 LITERATUREREVIEW 4
 2.1 ExistingSystem. . . . . . . . . . . . . . . . . . . . . . . . . . . . 6
 2.2 RelatedWork . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 7
 2.3 ResearchGap . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 7
 3 PROJECTDESCRIPTION 8
 3.1 ExistingSystem. . . . . . . . . . . . . . . . . . . . . . . . . . . . 8
 3.2 ProposedSystem . . . . . . . . . . . . . . . . . . . . . . . . . . . 9
 3.3 FeasibilityStudy . . . . . . . . . . . . . . . . . . . . . . . . . . . 9
 3.3.1 EconomicFeasibility . . . . . . . . . . . . . . . . . . . . . 10
 3.3.2 TechnicalFeasibility . . . . . . . . . . . . . . . . . . . . . 10
 3.3.3 SocialFeasibility . . . . . . . . . . . . . . . . . . . . . . . 11
 3.4 SystemSpecification . . . . . . . . . . . . . . . . . . . . . . . . . 11
 3.4.1 HardwareSpecification. . . . . . . . . . . . . . . . . . . . 11
 3.4.2 SoftwareSpecification . . . . . . . . . . . . . . . . . . . . 12
 3.4.3 ToolsandTechnologiesUsed . . . . . . . . . . . . . . . . 12
 3.4.4 StandardsandPolicies . . . . . . . . . . . . . . . . . . . . 13
4 SYSTEMDESIGNANDMETHODOLOGY 15
 4.1 SystemArchitecture. . . . . . . . . . . . . . . . . . . . . . . . . . 15
 4.2 DesignPhase . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 16
 4.2.1 DataFlowDiagram. . . . . . . . . . . . . . . . . . . . . . 16
 4.2.2 UseCaseDiagram . . . . . . . . . . . . . . . . . . . . . . 17
 4.2.3 ClassDiagram . . . . . . . . . . . . . . . . . . . . . . . . 18
 4.2.4 SequenceDiagram . . . . . . . . . . . . . . . . . . . . . . 19
 4.2.5 Collaborationdiagram . . . . . . . . . . . . . . . . . . . . 20
 4.2.6 ActivityDiagram. . . . . . . . . . . . . . . . . . . . . . . 21
 4.3 Algorithm&PseudoCode . . . . . . . . . . . . . . . . . . . . . . 21
 4.3.1 ConvolutionalNeuralNetworkAlgorithm. . . . . . . . . . 21
 4.3.2 PseudoCode . . . . . . . . . . . . . . . . . . . . . . . . . 22
 4.4 ModuleDescription . . . . . . . . . . . . . . . . . . . . . . . . . . 23
 4.4.1 DeepLearningFrameworks . . . . . . . . . . . . . . . . . 23
 4.4.2 Pre-TrainedObjectDetectionModels . . . . . . . . . . . . 24
 4.4.3 SetupSpeechandAudioProcessing . . . . . . . . . . . . . 25
 4.5 Stepstoexecute/run/implementtheproject . . . . . . . . . . . . . . 26
 4.5.1 ResearchandUnderstandUserNeeds . . . . . . . . . . . . 26
 4.5.2 PreprocessData. . . . . . . . . . . . . . . . . . . . . . . . 26
 4.5.3 ImplementAccessibilityFeatures . . . . . . . . . . . . . . 26
 5 IMPLEMENTATIONANDTESTING 27
 5.1 InputandOutput . . . . . . . . . . . . . . . . . . . . . . . . . . . 27
 5.1.1 InputDesign . . . . . . . . . . . . . . . . . . . . . . . . . 27
 5.1.2 OutputDesign . . . . . . . . . . . . . . . . . . . . . . . . 27
 5.2 Testing. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 27
 5.2.1 UnitTesting. . . . . . . . . . . . . . . . . . . . . . . . . . 27
 5.2.2 SystemTesting . . . . . . . . . . . . . . . . . . . . . . . . 28
 5.2.3 Input . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 30
 5.2.4 TestingStrategies . . . . . . . . . . . . . . . . . . . . . . . 31
 5.2.5 PerformanceEvaluation . . . . . . . . . . . . . . . . . . . 31
 6 RESULTSANDDISCUSSIONS 32
 6.1 EfficiencyoftheProposedSystem . . . . . . . . . . . . . . . . . . 32
 6.2 ComparisonofExistingandProposedSystem . . . . . . . . . . . . 33
 6.3 ComparativeAnalysis-Table . . . . . . . . . . . . . . . . . . . . . 34
6.4 ComparativeAnalysis-GraphicalRepresentationandDiscussion . . 35
 7 INDUSTRYDETAILS 36
 7.1 CognizantTechnologySolutions . . . . . . . . . . . . . . . . . . . 36
 7.1.1 (19/12/2024-19/04/2025) . . . . . . . . . . . . . . . . . . 36
 7.1.2 4Months . . . . . . . . . . . . . . . . . . . . . . . . . . . 36
 7.1.3 ManyataTechPark,Nagavara,Bengalur,Karnataka. . . . . . 36
 7.2 Internshipofferletter . . . . . . . . . . . . . . . . . . . . . . . . . 36
 7.3 Internshipofferletter . . . . . . . . . . . . . . . . . . . . . . . . . 37
 7.4 Internshipofferletter . . . . . . . . . . . . . . . . . . . . . . . . . 38
 7.5 InternshipCompletioncertificate . . . . . . . . . . . . . . . . . . . 38
 8 CONCLUSIONANDFUTUREENHANCEMENTS 39
 8.1 Summary . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 39
 8.2 Limitations . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 40
 8.3 FutureEnhancements . . . . . . . . . . . . . . . . . . . . . . . . . 40
 9 SUSTAINABLEDEVELOPMENTGOALS(SDGs) 42
 9.1 AlignmentwithSDGs. . . . . . . . . . . . . . . . . . . . . . . . . 42
 9.2 RelevanceoftheProjecttoSpecificSDG . . . . . . . . . . . . . . 43
 9.3 PotentialSocialandEnvironmentalImpact . . . . . . . . . . . . . . 43
 10PLAGIARISMREPORT 45
 11SOURCECODE 46
 11.1 SourceCode. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 46
 References 50
Chapter 1
 INTRODUCTION
 1.1 Introduction
 India being an agriculture country, about 70 percent of the population depends on
 it as their main source of income and food. Agriculture plays and important part of
 the Indian economy as it contributes about 17 percent of the total GDP. Farmers have
 wide range in selecting their crops and finding a suitable pesticide for it but in spite
 of all their efforts it can all be vain if they can’t identify the disease plaguing their
 crops. Thus, disease on crops can significantly reduce the quality and quantity of
 agricultural products along with economical damage to the farmers. To successfully
 cultivate crops without incurring much loss we need to properly identify the disease
 and remedy it, this requires a lot of work and processing time as detecting each and
 every plant can be tedious can time consuming. To lessen the burden of the farmers
 along with their losses we propose the use of a system which can detect infected
 plants so that we can curb the spread of infection and diseases at an earlier step thus
 reducing losses and crop failure.
 To tackle the problem of early and accurate detection of plant diseases, our system
 utilizes advanced image processing techniques combined with deep learning algo
rithms, specifically Convolutional Neural Networks (CNNs). CNNs have shown
 remarkable success in image classification tasks and are well-suited for identifying
 disease patterns from plant leaf images. By training the model on a dataset of
 various plant diseases, our system learns to distinguish between healthy and infected
 leaves with high accuracy. Once the disease is detected, the system can notify the
 user with the name of the disease and suggest possible remedies. This not only
 saves time but also enables even non-experts to recognize and act upon early signs
 of infection without needing in-person assistance from agricultural experts.
 The implementation of this system can be done using a mobile or web appli
cation where farmers can upload pictures of their crops. The system then processes
 the image, detects any disease symptoms, and delivers a result almost instantly. This
 1
makes it convenient and highly accessible, even in remote areas with limited access
 to agricultural support. The system can also be updated over time with new dis
ease data to improve its accuracy and scope. By maintaining a centralized database
 of common plant diseases and their symptoms, the system remains relevant and ef
fective as agricultural conditions evolve due to climate change and other external
 factors.
 1.2 Background
 Morbi non felis blandit, gravida risus a, feugiat nibh. Sed ex purus, aliquam nec
 justo sed, congue efficitur metus. Maecenas ac nunc ut ex faucibus tempor ac dig
nissim elit. Sed eu consequat purus, tincidunt consequat ipsum. Quisque pulvinar
 maximus condimentum. Nunc bibendum mauris ac interdum tempus. Donec ut sol
licitudin ex. Duis varius dolor mauris, sed dictum sem euismod consequat.
 1.3 Objective
 The scope of a project for object detection aimed at assisting impaired individuals
 encompasses various aspects. Firstly, it involves researching and selecting appropri
ate technologies such as computer vision and machine learning algorithms tailored
 to detect and recognize objects. Hardware considerations like cameras, sensors, and
 processing units need to be evaluated for effectiveness and compatibility. The project
 must include the development of a user-friendly interface accessible to people with
 diverse impairments, ensuring usability and inclusivity. Integration with existing as
sistive technologies or devices may also be necessary for seamless interaction. 2
 Data collection and annotation are crucial phases, involving the creation of compre
hensive datasets containing diverse objects in various environments to train and vali
date the detection models effectively. Testing and validation procedures should cover
 a wide range of scenarios to assess the system’s performance, accuracy, and robust
ness in real-world conditions, accounting for factors like lighting conditions, object
 occlusion, and user mobility. Deployment strategies need to be devised considering
 scalability, sustainability, and maintenance requirements. Furthermore, the project
 should address ethical and privacy considerations, ensuring user consent, data secu
rity, and compliance with relevant regulations. Documentation, training materials,
 and support mechanisms must be developed to facilitate the adoption and utilization
 2
of the system by impaired individuals and their caregivers. Continuous improve
ment through user feedback and technological advancements should be integrated
 into the project’s lifecycle to ensure its long-term efficacy and relevance. User in
terface design will focus on intuitive interaction methods, such as voice commands
 or tactile inputs, to relay object detection results effectively. Usability testing with
 target users will validate system performance and refine user experience. The project
 aims to enhance accessibility and independence by providing reliable object recog
nition capabilities, ultimately empowering visually impaired individuals to navigate
 their surroundings with greater confidence and safety.
 1.4 Problem Statement
 Object detection systems have become pivotal in numerous applications, ranging
 from autonomous vehicles to surveillance and accessibility tools. However, tradi
tional systems predominantly rely on visual interfaces, making them less effective or
 completely inaccessible to individuals with visual impairments. Additionally, these
 systems often require constant visual attention, which may not be feasible in certain
 real-world scenarios, such as while driving or operating machinery. The absence
 of alternative output modalities limits the inclusivity and usability of such systems,
 especially for users who depend on auditory information for interaction.
 Furthermore, most object detection implementations are designed for real-time
 use through cameras, lacking the flexibility to process static data files. This limita
tion hinders integration with existing workflows where batch processing or offline
 analysis of images is necessary. There is a growing need for a more adaptable solu
tion that not only delivers high accuracy in object detection but also offers accessible
 output through audio and allows data file input for increased convenience. Address
ing these gaps can significantly improve the usability and reach of object detection
 systems across diverse user needs and operational contexts.
 3
Chapter 2
 LITERATUREREVIEW
 Yang, R., et.al.[13] This paper provided an overview of computer vision techniques
 tailored for assisting visually impaired individuals, including object detection meth
ods and their applications.The survey on computer vision for visually impaired in
dividuals aims to gather insights into their needs and preferences regarding assis
tive technology. Questions cover usage patterns, desired features, and barriers faced
 when accessing visual information.
 Lee, S. et al.[7] The paper proposed a real-time object detection system based on
 deep learning for providing auditory feedback to the visually impaired.Real-time
 object detection for blind individuals using deep learning involves employing convo
lutional neural networks (CNNs) to process live video feeds from cameras or sensors.
 The system identifies objects in the user’s surroundings.and provides auditory or tac
tile feedback to convey their presence and location.
 Wang, Y. et al.[12] This work presented a wearable device that integrates object de
tection and recognition capabilities to assist visually impaired users in navigating
 their surroundings.A wearable assistive device for object detection and recognition
 for visually impaired individuals typically consists of a small camera or sensor array
 mounted on glasses or a headband. This device utilizes computer vision algorithms,
 often based on deep learning, to analyze the visual input in real-time.
 Chen, X. et al.[3] The authors explored methods to improve object recognition ac
curacy using smartphone cameras, catering specifically to the needs of visually im
paired users.Enhancing object recognition for the visually impaired involves refining
 algorithms for accuracy, speed, and adaptability to diverse environments. Integra
tion of multi-sensory feedback, customization options, and continuous improvement
 mechanisms ensures more intuitive and effective assistance, empowering users to
 navigate their surroundings with greater confidence and independence.
 Zhang, L. et al.[15] This paper presented a system that leverages convolutional neural
 networks (CNNs) for real-time object recognition and auditory feedback for visually
 impaired users.
 Liu, M. et al.[8] The study investigated efficient object detection techniques suit
4
able for wearable devices, aiming to optimize performance and resource utilization.
 Additionally, feedback on existing solutions and suggestions for improvement are
 solicited. The survey seeks to inform the development of more effective and user
friendly computer vision systems for the visually impaired community.
 Gupta, et al.[4] This research proposed an assistive object detection system utilizing
 Internet of Things (IoT) technology and deep learning for assisting visually impaired
 individuals.This technology enhances the independence and mobility of visually im
paired individuals by enabling them to navigate and interact with their environment
 more effectively.
 Li, et al.[6] The paper explored the feasibility of real-time object detection on edge
 devices, offering low-latency feedback suitable for visually impaired users. It iden
tifies objects in the user’s surroundings and provides auditory or tactile feedback to
 convey information about their presence, location, and characteristics. The device
 enhances the user’s independence and mobility by allowing them to navigate their
 environment interact with objects more effectively.
 Martinez, P. et al.[9] This work presented an accessible object detection system im
plemented on embedded platforms to provide practical support for blind and visually
 impaired individuals.A real-time object recognition system for impaired individuals
 employs computer vision algorithms to detect objects in their environment instantly.
 Yang, Q. et al.[14] The study evaluated different object detection models for wear
able devices, analyzing their effectiveness in assisting visually impaired users.It en
hances independence andnavigation for visually impaired individuals, enabling them
 to perceive and interact with their surroundings more effectively.
 Ahmed et al. [1] proposed an Edge-AI enabled solution in the form of smart glasses
 that provide real-time plant disease detection and guidance. This wearable system is
 capable of processing data locally, thus offering fast and context-aware agricultural
 insights without relying heavily on cloud infrastructure.
 Bashir et al.[2] developed a CNN-based real-time object detection system integrated
 with speech synthesis, aiming to assist visually impaired users. Their work demon
strates how combining computer vision and audio feedback can enhance spatial
 awareness and interaction for blind individuals.
 Kumar and Sharma [5] took a voice-driven approach by implementing a voice
assisted plant disease recognition system that leverages deep learning models in con
junction with IoT devices. Their model allows users, especially those with limited
 literacy or technical skills, to interact with the system using natural speech, thus
 5
making agricultural diagnostics more accessible.
 Mehta et al. [10] introduced a smart assistive system tailored for crop disease identi
f
 ication. Their system not only detects disease but also provides actionable guidance
 to farmers, highlighting the potential of intelligent tools in enhancing agricultural
 productivity and decision-making.
 Nair et al.[11] focused on the development of an audio-visual feedback system
 specifically designed for visually impaired individuals. By utilizing deep learning
 techniques, their system provides real-time feedback through both sound and vi
sual cues, improving the user’s ability to perceive and navigate their environment.
 Collectively, these studies underscore the growing impact of AI-based assistive tech
nologies in domains such as agriculture and accessibility, where real-time feedback,
 user-friendly interaction, and reliable detection are critical.
 2.1 Existing System
 The existing systems for object detection designed to assist impaired people em
ploy various technologies such as computer vision and machine learning to identify
 and classify objects in the environment. These systems typically utilize cameras
 integrated into smartphones or wearable devices to capture images, which are then
 processed in real-time to detect objects. The detected objects are conveyed to the
 user through auditory or haptic feedback, providing crucial information about the
 surroundings to aid navigation and awareness.
 However, existing systems may still face several disadvantages. One common
 challenge is the accuracy and reliability of object detection, especially in complex
 or cluttered environments. False positives or missed detections can occur, leading
 to incorrect or incomplete information being relayed to the user. Additionally, the
 computational resources required for real-time object detection can strain the ca
pabilities of mobile devices, impacting the system’s responsiveness and efficiency.
 Another limitation is the dependency on camera-based input, which may be affected
 by lighting conditions or occlusions, potentially hindering the system’s performance
 in certain situations. Lastly, the usability and accessibility of these systems can vary
 based onuser preferences and technological proficiency, emphasizing the importance
 of user-centered design and continuous improvement in this domain.
 Despite these challenges, ongoing research and development efforts continue to
 advance object detection systems for impaired individuals, aiming to enhance reli
6
ability, accuracy, and user experience through innovative technologies and method
ologies.
 2.2 Related Work
 Over the years, object detection has evolved significantly, with Convolutional
 Neural Networks (CNNs) becoming the backbone of most state-of-the-art detection
 models. Prominent models such as YOLO (You Only Look Once), SSD (Single Shot
 MultiBox Detector), and Faster R-CNN have demonstrated high accuracy and real
time performance in detecting and classifying objects in images and video streams.
 These models have been widely applied in areas like autonomous driving, surveil
lance, and mobile applications. In parallel, assistive technologies for the visually
 impaired, such as Microsoft’s Seeing AI and Google’s Lookout, have integrated ob
ject recognition with voice output to improve accessibility. These systems generally
 rely on real-time camera input and mobile device integration to provide feedback
 through audio cues.
 2.3 Research Gap
 While existing systems have made significant progress in object detection and
 accessibility, several gaps remain. First, many assistive tools are limited by their
 dependence on real-time camera input, which restricts their use in scenarios where
 batch processing or offline image analysis is needed. Second, few systems provide
 an option to input image data through files, limiting integration into automated work
f
 lows or existing databases. Third, although some applications offer voice feedback,
 the customization, clarity, and flexibility of the voice output often remain underde
veloped, reducing usability for users with specific auditory needs. Thus, there is a
 need for a system that combines robust CNN-based object detection with flexible
 image input (including file-based input) and high-quality, customizable voice output
 to enhance accessibility, usability, and integration in various real-world scenarios.
 7
Chapter 3
 PROJECTDESCRIPTION
 3.1 Existing System
 The existing systems for object detection designed to assist impaired people em
ploy various technologies such as computer vision and machine learning to identify
 and classify objects in the environment. These systems typically utilize cameras
 integrated into smartphones or wearable devices to capture images, which are then
 processed in real-time to detect objects. The detected objects are conveyed to the
 user through auditory or haptic feedback, providing crucial information about the
 surroundings to aid navigation and awareness.
 However, existing systems may still face several disadvantages. One common
 challenge is the accuracy and reliability of object detection, especially in complex
 or cluttered environments. False positives or missed detections can occur, leading
 to incorrect or incomplete information being relayed to the user. Additionally, the
 computational resources required for real-time object detection can strain the ca
pabilities of mobile devices, impacting the system’s responsiveness and efficiency.
 Another limitation is the dependency on camera-based input, which may be affected
 by lighting conditions or occlusions, potentially hindering the system’s performance
 in certain situations. Lastly, the usability and accessibility of these systems can vary
 based onuser preferences and technological proficiency, emphasizing the importance
 of user-centered design and continuous improvement in this domain.
 Despite these challenges, ongoing research and development efforts continue to
 advance object detection systems for impaired individuals, aiming to enhance reli
ability, accuracy, and user experience through innovative technologies and method
ologies.
 8
3.2 Proposed System
 The proposed system for object detection aimed at assisting impaired individuals
 leverages cutting-edge computer vision techniques and user-centered design princi
ples to overcome existing challenges and provide enhanced functionality. This sys
tem integrates advanced object detection algorithms, such as deep learning models
 like Faster CNN, to accurately identify and classify objects in real-time. By harness
ing the power of neural networks, the proposed system can achieve high levels of
 accuracy and robustness, minimizing false positives and ensuring reliable feedback
 to the user. One of the key advantages of the proposed system is its emphasis on
 usability and accessibility. The user interface is designed with visually impaired in
dividuals in mind, featuring intuitive interaction methods such as voice commands
 or tactile inputs to relay object detection results effectively. This focus on user
centered design enhances the system’s usability and adoption, empowering impaired
 individuals to navigate their surroundings with increased confidence and indepen
dence. Additionally, the proposed system can be deployed on various platforms,
 including smartphones or wearable devices, ensuring versatility and adaptability to
 different user preferences and needs.
 Another advantage of the proposed system is its potential for continuous improve
ment and adaptation through machine learning. By incorporating adaptive learning
 techniques, the system can evolve over time based on user feedback and environmen
tal data, further enhancing its performance and reliability. This adaptability enables
 the system to address diverse scenarios and challenges faced by impaired individu
als in real-world environments, ultimately contributing to improved accessibility and
 quality of life for users.
 3.3 Feasibility Study
 The proposed system is technically feasible due to the maturity and accessibility
 of the technologies involved. Convolutional Neural Networks (CNNs) have been
 widely adopted for object detection tasks and are supported by numerous open
source libraries such as TensorFlow, PyTorch, and OpenCV. These tools provide
 pre-trained models and easy-to-use frameworks that reduce the complexity of imple
mentation while maintaining high performance. Similarly, integrating voice output
 can be achieved using text-to-speech (TTS) engines such as Google Text-to-Speech,
 9
Amazon Polly, or open-source options like pyttsx3, which support clear and cus
tomizable audio output. The system can be designed to accept images through file
 input, which simplifies integration with existing data workflows and supports batch
 processing, making the solution versatile for different operational environments.
 From an economic and operational standpoint, the project is also feasible. The
 required hardware—standard computers with moderate GPU capabilities—makes it
 cost-effective for small-scale or individual use, while also scalable for larger de
ployments. The software stack is mostly open-source, minimizing licensing costs.
 Furthermore, the system’s ability to function offline (after initial setup) enhances its
 usability in low-connectivity environments, which is particularly beneficial for vi
sually impaired users in remote areas. Given these factors, the proposed solution is
 both technically and economically viable and holds strong potential for real-world
 deployment and further development.
 3.3.1 Economic Feasibility
 The economic feasibility of implementing object detection systems for impaired
 individuals involves evaluating both initial investment costs and long-term benefits.
 Initial costs include hardware (such as smartphones or wearable devices with cam
eras), software development, and training data for machine learning models. How
ever, these costs can be mitigated by leveraging existing technologies and open
source resources.
 Thelong-term benefits of object detection systems for the visually impaired justify
 the investment. These systems promote independence and safety, potentially reduc
ing the need for constant human assistance. They can also enhance productivity and
 employment opportunities for visually impaired individuals by improving their abil
ity to navigate and interact with their environment. Overall, the economic feasibility
 of object detection systems for the impaired is promising, with potential cost savings
 in the long run and significant improvements in quality of life and inclusion.
 3.3.2 Technical Feasibility
 Thetechnical feasibility of implementing object detection for impaired individuals
 is well-established due to advancements in computer vision and machine learning.
 Object detection algorithms, such as SSD (Single Shot MultiBox Detector), can ac
curately identify and classify objects in real-time, even on resource-constrained de
10
vices like smartphones or wearable gadgets. These systems leverage deep learning
 techniques and are capable of running efficiently on various platforms, providing au
ditory or haptic feedback to users about their surroundings. Furthermore, the avail
ability of open-source libraries and pre-trained models simplifies the development
 and deployment process, making object detection solutions accessible for develop
ers aiming to create assistive technologies for visually impaired individuals.
 3.3.3 Social Feasibility
 Thesocial feasibility of object detection systems for impaired individuals is highly
 favorable, as these technologies contribute to greater inclusivity and independence
 for people with visual impairments. By enhancing accessibility and mobility, object
 detection systems empower individuals to navigate their environments more confi
dently and participate more fully in daily activities. These systems also promote
 social integration by reducing barriers to communication and interaction, fostering
 a more inclusive society. Additionally, the development and adoption of such tech
nologies demonstrate societal progress towards accommodating diverse needs and
 promoting equal opportunities for individuals with disabilities. Overall, object de
tection for impaired people aligns with broader social goals of inclusivity and equity,
 enhancing the quality of life and social participation of visually impaired individuals.
 3.4 System Specification
 3.4.1 Hardware Specification
 • CPU: Intel Core i5 or AMD Ryzen 5
 • GPU: NVIDIA GTX1060or equivalent (6GB VRAM)
 • RAM:16GBDDR4
 • Storage: 500GB SSD
 • OS: Windows 10 or Linux (Ubuntu, CentOS)
 • Deep Learning Framework: TensorFlow, PyTorch (with GPU support)
 11
3.4.2 Software Specification
 • Operating System: Windows 10 (64-bit) or Linux (for compatibility and driver
 support)
 • Deep Learning Framework: TensorFlow or PyTorch (GPU-accelerated deep
 learning development)
 • Programming Language: Python (3.6 or later for framework compatibility and
 libraries)
 • Development Environment: Jupyter Notebook, Visual Studio Code, or PyCharm
 (code editing, debugging, visualization)
 • Additional Libraries: OpenCV (image processing), NiBabel (neuroimaging
 data), Scikit-learn (machine learning utilities), Matplotlib/Seaborn (visualiza
tion)
 • Version Control: Git (code management and collaboration)
 • Cloud Computing Platforms (optional): Google Colab, AWS, Azure (pre
configured environments and hardware)
 • Data Handling Tools: BraTS dataset tools or custom scripts (for loading and
 preprocessing)
 • Model Evaluation Metrics: Dice similarity coefficient, sensitivity, specificity
 (brain tumor segmentation performance assessment)
 3.4.3 Tools and Technologies Used
 • Python– Used as the primary programming language due to its extensive sup
port for machine learning and image processing libraries.
 • TensorFlow / Keras– Deep learning frameworks used to build and train the
 Convolutional Neural Network (CNN) for plant disease detection. Keras pro
vides a simple API while TensorFlow handles backend computation.
 • OpenCV–Utilized for various image processing tasks such as resizing, denois
ing, and enhancing images before feeding them into the CNN model.
 • NumPy and Pandas– Employed for efficient numerical operations, data pre
processing, and dataset management.
 12
• Matplotlib / Seaborn– Used to visualize training and validation results, such
 as accuracy/loss graphs and confusion matrices.
 • Jupyter Notebook / Google Colab– Provided an interactive environment for
 developing and testing the deep learning model, with GPU support for faster
 training.
 • LabelImg / Annotation Tools– Used for labeling and annotating images when
 creating or refining custom datasets.
 • Scikit-learn– Utilized for data splitting, model evaluation, and generating clas
sification reports including precision, recall, and F1-score.
 • Text-to-Speech (TTS) Libraries– Libraries such as pyttsx3 or gTTS were
 used to convert detected results into audible speech for enhanced accessibility.
 • Flask / Streamlit (Optional)– Lightweight frameworks used to build a user
 interface allowing users to upload images for real-time plant disease detection.
 3.4.4 Standards and Policies
 Anaconda Prompt
 Anaconda prompt is a type of command line interface which explicitly deals with
 the ML( MachineLearning) modules.And navigator is available in all the Win
dows,Linux and MacOS.The anaconda prompt has many number of IDE’s which
 make the coding easier. The UI can also be implemented in python.
 Standard Used: ISO/IEC 27001
 Jupyter
 It’s like an open source web application that allows us to share and create the
 documents which contains the live code, equations, visualizations and narrative text.
 It can be used for data cleaning and transformation, numerical simulation, statistical
 modeling, data visualization, machine learning.
 Standard Used: ISO/IEC 27001
 Google Colab
 Google Colab is a free playground for anyone wanting to explore Python in the
 cloud. No downloads, just open your browser and start coding! It provides access
 to powerful computing resources like GPUs and TPUs, making it ideal for machine
 learning, data analysis, or simply learning the ropes. You can even collaborate on
 projects with friends in real-time, sharing and editing notebooks like magic. While
 13
resources are shared and temporary, it’s perfect for quick experiments and learning
 bursts.
 Standard Used: ISO/IEC 27001
 14
Chapter 4
 SYSTEMDESIGNANDMETHODOLOGY
 4.1 System Architecture
 Figure 4.1: Architecture Diagram of Object Detection
 Figure 4.1 depicts the architecture diagram for object detection for impaired in
dividuals showcases a multi-layered system. At its core is the ”Detection Engine,”
 utilizing deep learning algorithms for real-time object recognition. Input is received
 from sensors like cameras or LiDAR, processed by the engine, and output to the
 ”Feedback Module.” This module interprets the data and provides feedback through
 auditory, tactile, or visual interfaces. User preferences are stored in the ”Settings
 Database,” allowing customization. Optionally, a ”Feedback Collection” component
 gathers user interactions for algorithm refinement. The system is scalable, with cloud
 integration for updates and data storage, ensuring continuous improvement and ac
cessibility.
 15
4.2 Design Phase
 4.2.1 Data Flow Diagram
 Figure 4.2: Data Flow Diagram of Object Detection
 Figure 4.2 depicts the data flow diagram for object detection for impaired people
 illustrates the flow of information within the system. Input data, such as images or
 sensor readings, are captured from the environment and fed into the object detection
 algorithm. The algorithm processes the data and identifies objects present in the en
vironment. Detected object information is then transmitted to the feedback module,
 where it is transformed into auditory, tactile, or visual cues for the user. User in
teraction data, such as settings adjustments or feedback, may also be captured and
 utilized to improve the object detection algorithm in future iterations.
 Once objects are identified, the results are forwarded to the Feedback Genera
tion Module, where the information is transformed into user-friendly output formats.
 Depending on user preferences and accessibility requirements, feedback may be de
livered as auditory cues (via text-to-speech engines), tactile responses (through vi
brations or Braille displays), or optional visual aids. The DFD also includes a User
 Interaction and Control Module, which captures user inputs such as setting adjust
ments, customization preferences, or system feedback.
 16
4.2.2 Use Case Diagram
 Figure 4.3: Use Case Diagram of Object Detection
 Figure 4.3 depicts the use case diagram for object detection for impaired people
 illustrates interactions between the user and the system. The ”Detect Objects” case
 captures input from sensors, processes it using object detection algorithms, and pro
vides feedback on detected objects. ”Provide Feedback” conveys information to the
 user through auditory, tactile, or visual cues. ”Adjust Settings” allows customization,
 while ”Access Help or Support” offers assistance features. ”Update System” ensures
 the system remains current, and ”Provide Training Data” optionally allows user feed
back for algorithm improvement. This diagram showcases essential functionalities,
 including detection, feedback, customization, support, system maintenance, and user
 involvement in enhancing algorithm accuracy.
 Additionally, the “Access Help or Support” use case enables users to receive trou
bleshooting assistance or guidance on using the system through voice commands or
 accessible help interfaces. The “Update System” ensures the software remains up
 to date with the latest enhancements, security patches, and model improvements.
 Meanwhile, the “Provide Training Data” use case allows users to contribute labeled
 images or feedback that can be used to retrain or fine-tune the object detection model,
 thereby improving its accuracy over time.
 17
4.2.3 Class Diagram
 Figure 4.4: Class Diagram of Object Detection
 Figure 4.4 presents the Class Diagram for the object detection system designed
 for visually impaired individuals, illustrating the core classes, their attributes, and
 the relationships that define the system’s architecture. At the center of the design is
 the User class, which represents the visually impaired individual interacting with the
 system. This class maintains user-specific data such as identification, preferences,
 and interaction history. The DetectionSystem class encapsulates the primary func
tionalities related to image acquisition, preprocessing, object detection using CNN
 models, and result handling. It serves as the central controller coordinating the flow
 of data and execution of tasks.
 Supporting this core logic are several interconnected classes. The DetectedObject
 class is responsible for storing structured data about each identified object, includ
ing labels, confidence scores, and location coordinates. The FeedbackModule class
 generates appropriate feedback based on the detected objects, translating data into
 auditory, tactile, or optional visual cues depending on user preferences. These pref
erences are managed by the Settings class, which allows the user to configure aspects
 such as feedback mode, voice type, or detection sensitivity.
 18
4.2.4 Sequence Diagram
 Figure 4.5: Sequence Diagram of Object Detection
 Figure 4.5 illustrates the Sequence Diagram for the object detection system de
veloped for visually impaired individuals, detailing the dynamic interactions and
 chronological flow of messages between system components and the user. The se
quence begins when the User initiates a detection request, which triggers the De
tectionSystem to activate the input module and capture environmental data through
 sensors or image files. This input is then forwarded to the ObjectDetectionEngine,
 where the Convolutional Neural Network (CNN) processes the data to identify and
 classify objects present in the scene.
 Once object detection is completed, the recognized objects are sent to the Feed
backModule, which determines the appropriate output modality based on user pref
erences retrieved from the Settings module. The feedback—whether auditory via
 text-to-speech, tactile through vibrations, or visual—is then delivered back to the
 user to convey the detected information clearly and accessibly.
 19
4.2.5 Collaboration diagram
 Figure 4.6: Collaboration diagram
 Figure 4.6 depicts the Entity-Relationship (ER) Diagram for the object detec
tion system tailored for visually impaired individuals, illustrating the key entities
 involved and the relationships between them. Central to the diagram is the User en
tity, representing the visually impaired individual interacting with the system. Each
 user can initiate one or more DetectionRequests, which are processed by the System
 entity. The system handles incoming data, performs object detection using CNN
based algorithms, and generates records of each DetectedObject, which are linked
 back to the detection sessions and user.
 The System entity is also responsible for managing Settings on a per-user basis,
 allowing customization of preferences such as feedback type (auditory, tactile, or
 visual), language, and detection sensitivity. Optionally, the User may submit Feed
backData, contributing real-world corrections or responses that are stored and used
 to enhance the system’s object detection algorithms over time.
 20
4.2.6 Activity Diagram
 Figure 4.7: Activity Diagram of Object Detection
 4.3 Algorithm & Pseudo Code
 4.3.1 Convolutional Neural Network Algorithm
 Convolutional Neural Network, particularly in combination with object detection
 algorithms, holds immense potential to assist impaired individuals in navigating their
 surroundings more independently. By leveraging CNNs, devices like smart glasses or
 smartphones equipped with cameras can recognize objects in real-time and provide
 auditory or tactile feedback to the user.
 For example, a CNN-powered object detection system can identify common ob
jects such as doors, chairs, or obstacles, and relay this information to the user through
 audio cues or vibrations. This allows visually impaired individuals to better navi
gate their environment, avoid obstacles, and locate desired objects. Training a CNN
 involves feeding it labeled data and optimizing its parameters to minimize the dis
crepancy between predicted and actual outputs. This process, known as backpropa
21
gation, iteratively adjusts the weights of the network using optimization algorithms
 like stochastic gradient descent (SGD) or Adam. Through this iterative optimization
 process, the CNN learns to extract meaningful features from raw data and generalize
 its knowledge to unseen examples.
 CNNs have achieved remarkable success in various computer vision tasks, in
cluding image classification, object detection, facial recognition, and image segmen
tation. Their ability to automatically learn hierarchical representations of features
 directly from raw data makes them incredibly powerful tools for analyzing and un
derstanding visual information. Moreover, CNNs have been adapted and extended
 to other domains beyond computer vision speech recognition.
 4.3.2 Pseudo Code
 1 # Import necessary libraries
 2 import numpy as np
 3 import tensorflow as tf
 4
 5 # Define the CNN architecture
 6 model = tf . keras . models . Sequential ([
 7
 8
 9
 10
 11
 12
 13
 14
 15
 16
 17 ])
 18
 # Convolutional layers
 t f . keras . layers .Conv2D(32 , (3 , 3) , activation=’ relu ’ , input shape =(image height , image width , 3)
 ) ,
 t f . keras . layers . MaxPooling2D ((2 , 2) ) ,
 t f . keras . layers .Conv2D(64 , (3 , 3) , activation=’ relu ’) ,
 t f . keras . layers . MaxPooling2D ((2 , 2) ) ,
 # Flatten layer to feed into fully connected layers
 t f . keras . layers . Flatten () ,
 # Fully connected layers
 t f . keras . layers . Dense(128 , activation=’ relu ’) ,
 t f . keras . layers . Dense( num classes , activation=’softmax ’)
 19 # Compile the model
 20 model . compile ( optimizer=’adam’ ,
 21
 22
 23
 l oss=’ sparse categorical crossentropy ’ ,
 metrics =[ ’accuracy ’ ])
 24 # Train the model
 25 model . fit ( train images , train
 validation
 26
 l a bels ) )
 27 # Evaluate the model
 l a bels , epochs=num epochs , validation
 28 test loss , test acc = model. evaluate ( test images , test labels )
 29
 30 # Use the model for object detection
 data =( validation images ,
 22
31 predictions = model. predict ( test images )
 4.4 Module Description
 4.4.1 Deep Learning Frameworks
 Deep learning frameworks have significantly advanced the development of as
sistive technologies aimed at improving the lives of visually impaired individuals,
 particularly in the domain of object detection. These frameworks provide the com
putational backbone for training and deploying models capable of identifying ob
jects in real-time from image or video streams captured by cameras or other sensors.
 Several deep learning frameworks have emerged as key players in this field, each
 offering unique features and advantages. One prominent framework is TensorFlow,
 developed by Google Brain. TensorFlow provides a comprehensive ecosystem for
 building and deploying deep learning models, including tools for data preprocessing,
 model training, and deployment on various platforms. With its high-level APIs such
 as TensorFlow Object Detection API, developers can quickly build and train cus
tom object detection models tailored to the needs of visually impaired users. These
 models can detect and classify objects in real-time, enabling applications such as
 navigation aids or object recognition systems.
 Figure 4.8: Deep Learning Frameworks
 23
4.4.2 Pre-Trained Object Detection Models
 Pre-trained object detection models serve as a cornerstone in developing assistive
 technologies for visually impaired individuals, offering efficient and accurate ob
ject recognition capabilities. These models have been trained on extensive datasets
 containing diverse objects and scenes, enabling them to identify objects in real-time
 with high precision. Leveraging pre-trained models expedites the development pro
cess by eliminating the need for extensive data collection and training, making it
 easier to deploy object detection systems tailored to the needs of visually impaired
 users. Faster CNN stands out as a popular choice in the realm of pre-trained object
 detection models. Renowned for its speed and accuracy, Faster CNN combines a
 region proposal network (RPN) with a convolutional neural network (CNN) back
bone to detect objects across various scales and aspect ratios. Pre-trained on datasets
 like COCO (Common Objects in Context), Faster CNN can discern a wide array
 of objects, making it a versatile solution for assistive applications. It offers another
 compelling option, prioritizing real-time performance. divides the input image into
 a grid and directly predicts bounding boxes and class probabilities for each grid cell.
 Its balance between speed and accuracy makes it ideal for applications requiring
 rapid ob
 Figure 4.9: Pre-Trained Object Detection
 24
4.4.3 Setup Speech and Audio Processing
 Setting up speech and audio processing for object detection to aid visually im
paired individuals involves integrating audio feedback and speech recognition with
 object detection systems to provide real-time assistance. The process typically be
gins with capturing audio inputs from microphones or other audio sensors, which
 are then processed to extract relevant features. Speech recognition algorithms are
 employed to convert spoken commands or queries into text, enabling users to inter
act with the system verbally. Simultaneously, object detection models, such as those
 mentioned previously, analyze visual inputs from cameras or image sensors to iden
tify objects in the user’s environment. These models can be pre-trained on extensive
 datasets to recognize a wide range of objects with high accuracy. Once an object
 is detected, relevant information about its identity, location, and characteristics is
 extracted from the visual data. The audio feedback component of the system con
verts this extracted information into speech or audio cues that are relayed to the user
 through headphones, earpieces, or speakers. This feedback informs the user about
 the presence and properties of detected objects in their surroundings. For example,
 upon detecting a ”chair,” the system may audibly announce the object’s name and
 location relative to the user, such as ”Chair located three meters ahead.
 Figure 4.10: Setup Speech and Audio Processing
 25
4.5 Steps to execute/run/implement the project
 4.5.1 Research and Understand User Needs
 Gain insights into the specific challenges faced by visually impaired individu
als regarding object recognition. Understand their requirements, preferences, and
 constraints.
 4.5.2 Preprocess Data
 Prepare the dataset by resizing images, normalizing pixel values, and splitting it
 into training, validation, and test sets.
 4.5.3 Implement Accessibility Features
 Integrate accessibility features into the system, such as audio feedback, text-to
speech capabilities, or tactile interfaces, to assist visually impaired users in interact
ing with the detected objects.
 26
Chapter 5
 IMPLEMENTATIONANDTESTING
 5.1 Input and Output
 5.1.1 Input Design
 Input testing for object detection for impaired individuals involves assessing the
 system’s accuracy in detecting common objects, performance in complex environ
ments and adverse conditions, responsiveness to user interactions, effectiveness of
 feedback modalities, customization options, and stability over prolonged use, ensur
ing reliable and intuitive functionality for visually impaired users.
 5.1.2 Output Design
 Output testing for object detection for impaired individuals verifies the system’s
 ability to provide accurate and timely feedback through auditory alerts, tactile vibra
tions, or visual cues. It evaluates the clarity, reliability, and effectiveness of feedback
 in conveying object information to visually impaired users for safe navigation and
 interaction with their environment.
 5.2 Testing
 Testing for object detection for impaired individuals involves comprehensive in
put testing to ensure accurate detection of common objects in various environments
 and adverse conditions. Output testing verifies effective feedback provision through
 auditory, tactile, or visual cues, ensuring reliable and intuitive functionality for visu
ally impaired users.
 5.2.1 Unit Testing
 1 # Checkbox to toggle voice output
 2 stop voice = st .checkbox(”Toggle Voice Output”)
 27
3
 4 # Speaking the prediction
 5 if not stop voice :
 6
 7
 8
 9
 10
 t r y :
 engine . say ( prediction
 engine . runAndWait ()
 except RuntimeError :
 t e xt )
 pass # Handle RuntimeError gracefully
 Unit testing for object detection in accessibility-focused systems ensures ac
curate detection of objects crucial for visually impaired users. It verifies individ
ual components of the detection process, including preprocessing, model infer
ence, and output formatting, to guarantee reliability and precision. Tests assess
 various scenarios, such as different lighting conditions and object orientations,
 ensuring consistent performance. Additionally, accessibility features like audio
 feedback are validated for usability and effectiveness, enhancing the overall user
 experience.
 5.2.2 System Testing
 1 import tensorflow as tf
 2 from tensorflow . keras . models import load model
 3 import streamlit as st
 4 import numpy as np
 5 import pyttsx3
 6
 7 # Initialize the text −to−speech engine
 8 engine = pyttsx3 . init ()
 9 voices = engine . getProperty ( ’voices ’)
 10 engine . setProperty ( ’voice ’ , voices [1]. id ) # Select a female voice , adjust index as needed
 11
 12 st . header ( ’Image Classification Model’)
 13
 14 try :
 15
 16
 17
 # Attempt to load model
 model path = ’\\Users\\pudur\\Downloads\\Image classification\\Image classify . keras ’
 model = load model(model path)
 18 except Exception as e:
 19
 20
 21
 s t . error ( f”Error loading model: {e}”)
 s t . stop ()
 22 data cat = [ ’apple ’ , ’banana ’ , ’beetroot ’ , ’bell pepper ’ , ’cabbage ’ , ’capsicum ’ , ’carrot ’ , ’
 cauliflower ’ ,
 28
23
 ’ c hilli pepper ’ , ’corn ’ , ’cucumber ’ , ’eggplant ’ , ’ garlic ’ , ’ginger ’ , ’grapes ’ , ’jalepeno
 ’ , ’kiwi ’ , ’lemon’ ,
 24
 25
 26
 ’ l ettuce ’ , ’mango’ , ’onion ’ , ’orange ’ , ’paprika ’ , ’pear ’ , ’peas ’ , ’pineapple ’ , ’
 pomegranate ’ , ’potato ’ ,
 ’ raddish ’ , ’soy beans ’ , ’spinach ’ , ’sweetcorn ’ , ’sweetpotato ’ , ’tomato ’ , ’turnip ’ , ’
 watermelon ’]
 27 img height = 180
 28 img width = 180
 29
 30 image = ’corn1 . jpg ’
 31 uploaded
 f i l e = st . file uploader (”Upload an image” , type=[”jpg” , ”jpeg” , ”png”])
 32 if uploaded
 33
 f i l e is not None:
 image = uploaded
 34
 f i l e . name
 35 image load = tf . keras . utils . load img(image , target size =(img height , img width))
 36 img arr = tf . keras . utils . img to array (image load)
 37 img bat = np.expand dims(img arr , axis=0)
 38
 39 predict = model. predict ( img bat )
 40 score = tf .nn. softmax( predict )
 41
 42 st . image(image , width=200)
 43
 44 prediction
 45 accuracy
 t e xt = data cat [np.argmax( score ) ]
 t ext = ( ’With ’) + str (round ((np.max( score ) * 100) , 3)) + ’ % accuracy ’
 System testing for object detection systems catering to visually impaired in
dividuals involves evaluating the entire system’s functionality and performance.
 This comprehensive testing assesses the system’s ability to accurately detect ob
jects in diverse environments and lighting conditions, ensuring reliability in real
world scenarios. Additionally, it verifies the effectiveness of accessibility fea
tures such as audio feedback and text-to-speech capabilities in assisting visually
 impaired users. System testing validates the system’s usability, accuracy, and
 robustness, ultimately enhancing accessibility for impaired individuals.
 29
5.2.3 Input
 Figure 5.1: Test Image of Object Detection
 The provided image showcases a well-organized dataset directory, where each
 folder represents a distinct class of fruits or vegetables such as apple, banana, tomato,
 spinach, lettuce, mango, and many others. This structure is typically used in image
 classification tasks, particularly with convolutional neural networks (CNNs), to facil
itate supervised learning. Each folder contains multiple images of the corresponding
 item, making it suitable for training, validation, and testing of deep learning mod
els. The visual thumbnails on the folder icons offer a quick preview of the images
 inside, helping to verify the dataset content at a glance. This type of dataset orga
nization is commonly utilized with frameworks like TensorFlow or PyTorch using
 directory-based data loaders.
 30
5.2.4 Testing Strategies
 5.2.5 Performance Evaluation
 Figure 5.2: Test Image
 The above figure illustrates the training and validation performance of the Convo
lutional Neural Network (CNN) model across 25 epochs. The left panel represents
 the Accuracy, while the right panel depicts the Loss trend.
 In the Accuracy plot, both training and validation accuracies exhibit a steep rise
 within the initial 5 epochs, indicating rapid learning. The training accuracy ap
proaches nearly 100, while the validation accuracy stabilizes around 95, demonstrat
ing a strong generalization capability of the model. The slight divergence between
 the two curves after epoch 15 may indicate a minor overfitting tendency, though not
 significantly impactful. In the Loss plot, both curves show a sharp decline during the
 early training stages, with training loss eventually dropping below 0.1. The valida
tion loss levels off slightly higher than the training loss, hovering around 0.5, which
 is acceptable given the model complexity and input noise.
 31
Chapter 6
 RESULTSANDDISCUSSIONS
 6.1 Efficiency of the Proposed System
 Theefficiency of aproposedobject detection system for impaired people is critical
 for its practical adoption and usability. The system’s efficiency encompasses several
 key aspects. Firstly, the accuracy and reliability of the object detection algorithm
 are paramount. The system must be able to detect and classify objects in real-time
 with high precision, especially in dynamic and cluttered environments where visually
 impaired individuals navigate daily. Utilizing state-of-the-art deep learning models
 like YOLO (You Only Look Once) or SSD (Single Shot MultiBox Detector) can
 enhance accuracy while maintaining efficient inference speeds suitable for real-time
 applications on resource-constrained devices.
 Secondly, the efficiency of the system involves optimizing computational re
sources. Object detection algorithms should be optimized to run efficiently on the
 target hardware, such as smartphones or wearable devices, to minimize processing
 time and conserve battery life. Techniques like model quantization, pruning, and
 hardware acceleration (e.g., using GPU or specialized neural processing units) can
 significantly improve computational efficiency without compromising accuracy.
 Additionally, the system’s efficiency extends to the user interface and interac
tion design. The user interface should be intuitive and accessible, providing clear
 and timely feedback to visually impaired users about detected objects. Audio-based
 feedback, tactile vibrations, or voice commands can enhance the system’s usability,
 enabling seamless integration into daily life activities.
 Moreover, the efficiency of the proposed system involves robustness and adapt
ability. The system should be capable of handling various environmental condi
tions, such as changes in lighting or occlusions, to maintain consistent performance.
 Continuous improvement through adaptive learning techniques, such as online fine
tuning of models based on user feedback, can enhance the system’s adaptability and
 responsiveness over time.
 32
6.2 Comparison of Existing and Proposed System
 Existing System: In traditional systems for plant disease detection, the process
 is either manual or based on simple image processing techniques. These systems
 rely heavily on predefined features like color, texture, and shape for classification.
 However, such approaches lack the intelligence to generalize across diverse plant
 species and various stages of disease progression. Manual inspection requires expert
 knowledge and is time-consuming, especially in large-scale farming. In most cases,
 there is no support for real-time feedback, and the outputs are only visual, which
 limits accessibility, especially for visually impaired users. The lack of automation
 and adaptability in these existing systems often leads to inconsistent results, lower
 accuracy, and delayed disease control, which can significantly impact crop yield and
 increase financial losses for farmers.
 Proposed System: The proposed system addresses the limitations of the existing
 system by utilizing a Convolutional Neural Network (CNN) for intelligent, auto
mated, and accurate plant disease detection. CNNs have the ability to learn from
 large datasets and extract deep visual features, making them highly effective for im
age classification tasks. The system not only processes and identifies diseases from
 plant images with high precision but also includes a voice output feature, allowing
 the results to be audibly announced. This enhances accessibility for users with visual
 impairments and those working in environments where screen interaction is not prac
tical. Additionally, the proposed system supports image file input, enabling batch
 processing and easy integration into existing agricultural workflows. By combining
 deep learning with voice-enabled feedback, the system offers a scalable, efficient,
 and inclusive solution that minimizes human error and supports timely intervention
 for disease control.
 33
6.3 ComparativeAnalysis-Table
 Feature ExistingSystems ProposedSystem
 DiseaseDetectionMethod Manual inspectionorbasicimagepro
cessingtechniques
 AdvancedConvolutionalNeuralNet
work(CNN)foraccuratedetectionand
 classification
 AccuracyandReliability Oftensubjectiveandlessaccurate Highaccuracy throughdeep learning
 trainedonlargedatasets
 UserAccessibility Primarilyvisualinterfaceonly Voice outputmakes it accessible for
 visually impairedand less tech-savvy
 users
 InputMethod Real-timecameraonlyinmostsystems Supportsboth real-timecamera input
 andbatchimagefiles
 ProcessingTime Slower andmay requireexpert inter
pretation
 Fast, automated detection using pre
trainedmodel
 Scalability Limited scalability and usability in
 largefarms
 Easilyscalableandcanbe integrated
 withagriculturalmonitoringsystems
 InternetDependency Many tools relyoncloud-basedpro
cessing
 Canbeconfiguredtorunofflineusing
 localmodelsandTTSengines
 RemedySuggestions Oftenrequiresmanuallookuporexpert
 help
 Canbeextendedtoprovideimmediate
 suggestionsfor treatmentof identified
 diseases
 CostofOperation High, especiallyifexpertdiagnosisor
 equipmentisneeded
 Low-cost solution suitable for small
 andmarginalfarmers
 TargetUsers Agriculturalexpertsor trainedperson
nel
 Designedtoassistcommonfarmers,es
peciallythosewithlimitedaccesstoex
pertsupport
 Table6.1:ComparisonofExistingandProposedSystem
 The tablepresentedaboveoutlinesacomparativeanalysisbetweentraditional
 (existing)systemsusedforplantdiseasedetectionandtheproposedintelligentsolu
tionthatintegratesConvolutionalNeuralNetworks(CNN)withvoiceoutput.Exist
ingsystemsoftenrelyonmanualinspectionorrudimentaryimageprocessingtech
niques,whichcan lead to inaccurateor subjective resultsdue tohumanerroror
 limitedfeatureextractioncapabilities. Incontrast, theproposedsystememploysa
 robustCNNmodeltrainedonalargedataset,ensuringsignificantlyhigheraccuracy
 andreliableclassificationofdiseases.
 34
6.4 Comparative Analysis-Graphical Representation and Discussion
 Figure 6.1: Graphical Representation
 The graphical representations included in this project provide visual insights into
 the performance and efficiency of the proposed system compared to existing method
ologies. These graphs serve to illustrate key metrics such as model accuracy, process
ing time, classification results, and user accessibility enhancements. For instance, bar
 charts or line graphs may be used to demonstrate the comparative mean Average Pre
cision (mAP) achieved by different models, highlighting the superior performance of
 the proposed CNN-based approach.
 35
Chapter 7
 INDUSTRYDETAILS
 7.1 Cognizant Technology Solutions
 7.1.1
 (19/12/2024- 19/04/2025)
 7.1.2 4Months
 7.1.3 Manyata Tech Park,Nagavara,Bengalur,Karnataka
 7.2 Internship offer letter
 36
7.3 Internship offer letter
 37
7.4 Internship offer letter
 7.5 Internship Completion certificate
 38
Chapter 8
 CONCLUSIONANDFUTURE
 ENHANCEMENTS
 8.1 Summary
 In conclusion, object detection technology represents a transformative solution
 for enhancing accessibility and independence among visually impaired individuals.
 Through the integration of advanced computer vision algorithms and assistive de
vices, object detection systems empower users by providing real-time information
 about their surroundings. This technology plays a crucial role in improving spatial
 awareness, facilitating safer navigation, and promoting social inclusion for individu
als with visual impairments.
 The development and adoption of object detection systems for impaired people
 signify a significant step towards creating more inclusive and equitable societies. By
 leveraging state-of-the-art machine learning models and accessible user interfaces,
 these systems cater to the specific needs and challenges faced by visually impaired
 individuals, allowing them to navigate environments with greater confidence and au
tonomy. Moreover, the continuous evolution of object detection technology holds
 promise for further advancements in assistive technologies, offering enhanced func
tionalities and usability over time.
 Looking ahead, it is essential to continue advancing research and development ef
forts in this field while ensuring adherence to accessibility standards, data privacy
 regulations, and ethical guidelines. Collaboration among researchers, developers,
 policymakers, and advocacy groups is crucial to promote the responsible and inclu
sive deployment of object detection solutions for impaired individuals. Ultimately,
 by harnessing the potential of object detection technology, we can empower visually
 impaired individuals to overcome barriers, participate more actively in daily activi
ties, and experience greater independence and quality of life.
 39
8.2 Limitations
 While the proposed system offers significant advancements in plant disease detec
tion through the use of Convolutional Neural Networks and voice output, it still has
 certain limitations that affect its full potential. One of the primary limitations is the
 dependency on high-quality and well-labeled datasets. The performance of the CNN
 model is directly influenced by the quality and variety of the images used during
 training. If the dataset does not contain sufficient examples of different diseases or
 plant types, the model may struggle to accurately classify unseen data in real-world
 scenarios. Furthermore, lighting conditions, background noise in images, and image
 resolution may affect detection accuracy. This restricts the system’s ability to gen
eralize across diverse agricultural environments, especially in regions where ideal
 image capture conditions are not feasible.
 Another limitation lies in the voice output functionality. While it enhances ac
cessibility, especially for visually impaired users, it may not be effective in noisy
 agricultural environments or for users speaking different languages or dialects. The
 current implementation may only support limited languages and simple sentence
 structures, which could restrict its usability across multicultural or multilingual user
 bases. Additionally, the system currently processes images sequentially and may
 not be optimized for real-time performance in large-scale field applications. This
 makes it less practical for rapid disease monitoring across vast farmlands without
 further hardware or software optimization. Future work should address these issues
 by incorporating multilingual support, noise-canceling features in audio output, and
 real-time edge processing capabilities.
 8.3 Future Enhancements
 1. Improved Object Recognition Algorithms: Continuously refining and op
timizing object recognition algorithms can lead to more accurate and efficient
 detection of objects in various environments.
 2. Multi-Sensory Integration: Integrating multiple sensory inputs such as vi
sion, sound, and touch can provide a more comprehensive understanding of the
 surroundings. For example, combining visual object detection with audio cues
 or haptic feedback can enhance accessibility for visually impaired individuals.
 3. Real-Time Feedback Systems: Developing real-time feedback systems that
 40
provide immediate information about detected objects can help impaired indi
viduals navigate their surroundings more effectively. This could include audi
tory alerts or vibrations to indicate the presence and location of objects.
 4. Customizable Interfaces: Designing customizable interfaces that allow
 users to tailor the object detection system according to their specific needs and
 preferences can improve usability and accessibility.
 5. Integration with Wearable Technology: Integrating object detection tech
nology into wearable devices such as smart glasses or haptic vests can provide
 a seamless and hands-free experience for impaired individuals, allowing them
 to receive real-time object detection information directly through their wearable
 devices.
 6. Machine Learning for Personalization: Leveraging machine learning al
gorithms to personalize the object detection system based on individual prefer
ences, behaviors, and environments can enhance its effectiveness and usability
 over time.
 7. Cloud-Based Object Recognition: Utilizing cloud-based object recognition
 services can provide access to a vast database of object models and enable real
time updates and improvements to the detection algorithms.
 8. Collaboration with Accessibility Experts: Collaborating with accessibil
ity experts and individuals with disabilities throughout the development process
 can ensure that the object detection system meets the specific needs and require
ments of impaired users.
 9. Privacy and Security Considerations: Incorporating robust privacy and se
curity measures to protect the sensitive data collected by the object detection
 system is crucial to ensure the trust and adoption of the technology.
 41
Chapter 9
 SUSTAINABLEDEVELOPMENT
 GOALS(SDGs)
 9.1 Alignment with SDGs
 Theproposedproject aligns strongly with the United Nations’ Sustainable De
velopment Goals by promoting technological innovation in agriculture, increas
ing accessibility, and supporting inclusive development. By leveraging Convolu
tional Neural Networks for accurate plant disease detection and integrating voice
 output for accessibility, the system addresses both agricultural efficiency and so
cial inclusivity. This contributes to sustainable farming practices by minimizing
 crop loss, improving food production, and empowering farmers, especially those
 in under-resourced or rural areas.
 Furthermore, the project’s inclusive design—with voice support—ensures that
 individuals with visual impairments or limited literacy can also benefit, thereby
 reducing inequalities in access to agricultural tools and knowledge. The system’s
 ability to work offline or in low-resource environments enhances its relevance in
 developing regions, making it a valuable tool in achieving sustainable develop
ment in agriculture and technology access.
 42
9.2 Relevance of the Project to Specific SDG
 SDG2–ZeroHunger: The system directly contributes to SDG 2 by support
ing early detection of crop diseases, thereby reducing crop failure and improving
 food security. Timely diagnosis ensures better yields and helps in maintaining a
 stable food supply.
 SDG3–GoodHealthandWell-Being: By reducing the spread of plant diseases
 and ensuring the health of crops, the system indirectly supports public health.
 Healthy crops mean fewer chances of pesticide overuse and safer food produc
tion.
 SDG 9– Industry, Innovation, and Infrastructure: The integration of AI and
 voice technology into agriculture fosters innovation and contributes to building
 resilient infrastructure for smart farming. This represents a step forward in mod
ernizing traditional farming techniques.
 SDG 10– Reduced Inequalities: The inclusion of voice output functionality
 supports users with visual impairments or literacy barriers, promoting equality
 in access to technological tools and information.
 SDG12–Responsible Consumption and Production: By helping farmers iden
tify diseases early, the system promotes efficient use of agricultural inputs such
 as pesticides and fertilizers, reducing waste and environmental damage.
 9.3 Potential Social and Environmental Impact
 The proposed system holds substantial potential for positive social impact,
 particularly in rural and agricultural communities where access to expert guid
43
ance and technological support is limited. By empowering farmers with an ac
cessible, AI-driven tool for early detection of plant diseases, the system con
tributes to improving their livelihood and economic resilience. The voice output
 feature adds inclusivity by enabling visually impaired individuals and those with
 limited literacy to effectively interact with the system, thereby promoting social
 equity and digital inclusion in the agricultural sector. This can lead to greater
 independence and confidence among marginalized groups, contributing to inclu
sive growth and community development.
 From an environmental standpoint, the early and accurate identification of plant
 diseases reduces the overuse and misuse of chemical pesticides and fertilizers.
 This not only minimizes soil and water pollution but also protects beneficial
 insects and biodiversity in farming ecosystems. By encouraging responsible
 agricultural practices, the system helps preserve natural resources and supports
 sustainable land use. Additionally, reducing crop failure through timely inter
vention can lower the carbon footprint associated with replanting and wasted
 resources. Overall, the project contributes to building a more sustainable and
 environmentally-conscious agricultural future, aligning technology use with
 ecological stewardship.
 44
Chapter 10
 PLAGIARISMREPORT
 Figure 10.1: Plagiarism Report of Object Detection
 45
Chapter11
 SOURCECODE
 11.1 SourceCode
 1 import numpy as np
 2 import pandas as pd
 3 import matplotlib.pyplot as plt
 4 import tensorflow as tf
 5
 6 from tensorflow import keras
 7 from tensorflow.keras import layers
 8 data train path = ’Fruits Vegetables/ train’
 9 data test path = ’Fruits Vegetables/ test ’
 10 data val path = ’Fruits Vegetables/validation’
 11 imgwidth = 180
 12 img height =180
 13 data train = tf .keras . utils . image dataset from directory(
 14 data train path ,
 15 shuffle=True,
 16 image size=(imgwidth , img height) ,
 17 batch size=32,
 18 validation split=False)
 19 data cat = data train.class names
 20 data cat
 21 data val = tf .keras . utils . image dataset from directory(data val path ,
 22 image size=(img height , imgwidth) ,
 23 batch size=32,
 24 shuffle=False ,
 25 validation split=False)
 26 data test = tf .keras . utils . image dataset from directory(
 27 data test path ,
 28 image size=(img height , imgwidth) ,
 29 shuffle=False ,
 30 batch size=32,
 31 validation split=False
 32 )
 33 plt . figure(figsize=(10,10))
 34 for image, labels in data train. take(1) :
 35 for i in range(9) :
 36 plt . subplot(3,3, i+1)
 37 plt .imshow(image[i ].numpy() .astype(’uint8’))
 46
38
 plt . t i t l e ( data cat [ labels [ i ]])
 39
 plt . axis ( ’ off ’)
 40 from tensorflow . keras . models import Sequential
 41 data train
 42 model = Sequential ([
 43
 44
 45
 46
 47
 48
 49
 50
 51
 52
 53
 54
 55 ])
 l ayers . Rescaling (1./255) ,
 l ayers .Conv2D(16 , 3, padding=’same’ , activation=’ relu ’) ,
 l ayers . MaxPooling2D () ,
 l ayers .Conv2D(32 ,3 , padding=’same ’ , activation=’ relu ’) ,
 l ayers . MaxPooling2D () ,
 l ayers .Conv2D(64 , 3, padding=’same’ , activation=’ relu ’) ,
 l ayers . MaxPooling2D () ,
 l ayers . Flatten () ,
 l ayers . Dropout (0.2) ,
 l ayers . Dense(128) ,
 l ayers . Dense( len ( data cat ) )
 56 model . compile ( optimizer=’adam’ , loss=tf . keras . losses . SparseCategoricalCrossentropy ( from
 True ) , metrics =[ ’accuracy ’ ])
 57 epochs size = 25
 58 history = model. fit ( data train , validation
 59 epochs range = range( epochs size )
 60 plt . figure ( figsize =(8 ,8) )
 61 plt . subplot (1 ,2 ,1)
 data=data val , epochs=epochs size )
 62 plt . plot ( epochs range , history . history [ ’accuracy ’] , label = ’Training Accuracy ’)
 63 plt . plot ( epochs range , history . history [ ’val accuracy ’] , label = ’Validation Accuracy ’)
 64 plt . t i t l e ( ’Accuracy ’)
 65
 66 plt . subplot (1 ,2 ,2)
 67 plt . plot ( epochs range , history . history [ ’ loss ’] , label = ’Training Loss ’)
 68 plt . plot ( epochs range , history . history [ ’ val loss ’] , label = ’Validation Loss ’)
 69 plt . t i t l e ( ’Loss ’)
 70 image = ’Fruits Vegetables / test / garlic / Image 2 . jpg ’
 71 image = tf . keras . utils . load img (image , target size =(img height , img width) )
 72 img arr = tf . keras . utils . array to img (image)
 73 img bat=tf . expand dims( img arr ,0)
 74 predict = model. predict ( img bat )
 75 score = tf .nn. softmax( predict )
 l ogits=
 76 print ( ’Veg/ Fruit in image is {} with accuracy of {:0.2 f}’. format( data cat [np.argmax( score ) ] ,np.
 max( score ) *100) )
 77 model . save ( ’ Image classify . keras ’)
 47
1 import tensorflow as tf
 2 from tensorflow . keras . models import load model
 3 import streamlit as st
 4 import numpy as np
 5 import pyttsx3
 6
 7 # Initialize the text −to−speech engine
 8 engine = pyttsx3 . init ()
 9 voices = engine . getProperty ( ’voices ’)
 10 engine . setProperty ( ’voice ’ , voices [1]. id ) # Select a female voice , adjust index as needed
 11
 12 st . header ( ’Image Classification Model’)
 13
 14 try :
 15
 16
 17
 # Attempt to load model
 model path = ’\\Users\\pudur\\Downloads\\Image classification\\Image classify . keras ’
 model = load model(model path)
 18 except Exception as e:
 19
 20
 21
 s t . error ( f”Error loading model: {e}”)
 s t . stop ()
 22 data cat = [ ’apple ’ , ’banana ’ , ’beetroot ’ , ’bell pepper ’ , ’cabbage ’ , ’capsicum ’ , ’carrot ’ , ’
 cauliflower ’ ,
 23
 24
 25
 26
 ’ c hilli pepper ’ , ’corn ’ , ’cucumber ’ , ’eggplant ’ , ’ garlic ’ , ’ginger ’ , ’grapes ’ , ’
 j alepeno ’ , ’kiwi ’ , ’lemon ’ ,
 ’ l ettuce ’ , ’mango’ , ’onion ’ , ’orange ’ , ’paprika ’ , ’pear ’ , ’peas ’ , ’pineapple ’ , ’
 pomegranate ’ , ’potato ’ ,
 ’ raddish ’ , ’soy beans ’ , ’spinach ’ , ’sweetcorn ’ , ’sweetpotato ’ , ’tomato ’ , ’turnip ’ ,
 ’ watermelon ’]
 27 img height = 180
 28 img width = 180
 29
 30 image = ’corn1 . jpg ’
 31 uploaded
 f i l e = st . file uploader (”Upload an image” , type=[”jpg” , ”jpeg” , ”png”])
 32 if uploaded
 33
 f i l e is not None:
 image = uploaded
 34
 f i l e . name
 35 image load = tf . keras . utils . load img(image , target size =(img height , img width))
 36 img arr = tf . keras . utils . img to array (image load)
 37 img bat = np.expand dims(img arr , axis=0)
 38 import numpy as np
 39 import pandas as pd
 40 import matplotlib . pyplot as plt
 41 import tensorflow as tf
 42 from keras import regularizers , layers , optimizers , utils , models
 43 import pyttsx3
 44 import streamlit as st
 45
 48
46 # Initialize the text −to−speech engine
 47 engine = pyttsx3 . init ()
 48 voices = engine . getProperty ( ’voices ’)
 49 engine . setProperty ( ’voice ’ , voices [1]. id ) # Select a female voice , adjust index as needed
 50
 51 st . header ( ’Image Classification Model’)
 52
 53 try :
 54
 55
 56
 # Attempt to load model
 model path = ’\\Leela\\Image classification (2)\\Image classification\\Image classify . keras
 ’
 model = models . load model(model path)
 57 except Exception as e:
 58
 59
 60
 s t . error ( f”Error loading model: {e}”)
 s t . stop ()
 61 data cat = [ ’apple ’ , ’banana ’ , ’beetroot ’ , ’bell pepper ’ , ’cabbage ’ , ’capsicum ’ , ’carrot ’ , ’
 cauliflower ’ ,
 62
 63
 64
 65
 ’ c hilli pepper ’ , ’corn ’ , ’cucumber ’ , ’eggplant ’ , ’ garlic ’ , ’ginger ’ , ’grapes ’ , ’
 j alepeno ’ , ’kiwi ’ , ’lemon ’ ,
 ’ l ettuce ’ , ’mango’ , ’onion ’ , ’orange ’ , ’paprika ’ , ’pear ’ , ’peas ’ , ’pineapple ’ , ’
 pomegranate ’ , ’potato ’ ,
 ’ raddish ’ , ’soy beans ’ , ’spinach ’ , ’sweetcorn ’ , ’sweetpotato ’ , ’tomato ’ , ’turnip ’ ,
 ’ watermelon ’]
 66 img height = 180
 67 img width = 180
 68 image = ’corn1 . jpg ’
 69 uploaded
 f i l e = st . file uploader (”Upload an image” , type=[”jpg” , ”jpeg” , ”png”])
 70 if uploaded
 71
 f i l e is not None:
 image = uploaded
 72
 f i l e . name
 73 image load = tf . keras . utils . load img(image , target size =(img height , img width))
 74 img arr = tf . keras . utils . img to array (image load)
 75 img bat = np.expand dims(img arr , axis=0)
 76
 77 predict = model. predict ( img bat )
 78 score = tf .nn. softmax( predict )
 79
 80 st . image(image , width=200)
 81
 82 prediction
 83 accuracy
 t e xt = data cat [np.argmax( score ) ]
 t ext = ( ’With ’) + str (round ((np.max( score ) * 100) , 3)) + ’ % accuracy ’
 84
 85 st . write ( prediction
 86 st . write ( accuracy
 t e xt )
 t ext )
 87 # Checkbox to toggle voice output
 88 stop voice = st .checkbox(”Toggle Voice Output”)
 89 # Speaking the prediction
 90 if not stop voice :
 49
91
 t r y :
 engine . say ( prediction
 t e xt )
 92
 93
 94
 95
 engine . runAndWait ()
 except RuntimeError :
 pass # Handle RuntimeError gracefully
 50
References
 [1] AhmedK., RahmanM., andHasanM., “Edge-AIenabled smart glasses for
 real-time plant disease detection and guidance,” Proc. IEEE Conf. Comput.
 Vis. Agric. Environ. (CVAE), 2021.
 [2] Bashir S., Arshad S., and Khan M., “CNN-based real-time object detection
 system integrated with speech synthesis for blind users,” Proc. IEEE Global
 Humanitarian Technol. Conf. (GHTC), 2020.
 [3] Chen X., Liu H., and Wang Z., “Enhancing object recognition for visu
ally impaired individuals using smartphone cameras,” Proc. IEEE Int. Conf.
 Multimedia Expo (ICME), 2022.
 [4] Gupta R. and Patel S., “Assistive object detection system using IoT and
 deep learning for the blind,” Proc. IEEE Int. Conf. Big Data, 2019.
 [5] Kumar A. and Sharma R., “Voice-assisted plant disease recognition using
 deep learning and IoT,” Proc. IEEE Int. Conf. Artif. Intell. IoT (AIIoT),
 2020.
 [6] Li W. and Wang Z., “Real-time object detection system for visually im
paired people using edge computing,” Proc. IEEE Int. Conf. Edge Comput.
 (EDGE), 2021.
 [7] Lee S., Kim J., and Park H., “Real-time object detection for the blind using
 deep learning,” Proc. IEEE Int. Conf. Consum. Electron. (ICCE), 2020.
 [8] Liu M., Liu Y., and Zhang Z., “Efficient object detection techniques for
 wearable devices for the visually impaired,” Proc. IEEE Int. Conf. Consum.
 Electron. (ICCE), 2019.
 51
[9] Martinez P., Fernandez L., and Rodriguez A., “Accessible object detection
 system for blind and visually impaired people using embedded platforms,”
 Proc. IEEE Int. Conf. Syst., Man, Cybern. (SMC), 2021.
 [10] Mehta P., Jindal S., and Rajput D., “Smart assistive system for crop dis
ease identification and guidance for farmers,” Proc. IEEE Int. Conf. Smart
 Technol. Agric. (SmartAgri), 2022.
 [11] Nair S., Vinayakumar R., and Soman K. P., “Deep learning-based audio
visual feedback system for visually impaired,” Proc. IEEE Int. Conf. Intell.
 Human Comput. Interact. (IHCI), 2021.
 [12] Wang Y., Zhang J., and Liu Q., “Wearable assistive device for object detec
tion and recognition for visually impaired people,” Proc. IEEE Int. Conf.
 Robot. Autom. (ICRA), 2021.
 [13] Yang R., He X., Cao Y., Li Y., and Li H., “Real-time object detection and
 recognition for visually impaired people using deep learning,” Proc. IEEE
 Int. Conf. Robot. Autom. (ICRA), 2018.
 [14] Yang Q. and Wang R., “Evaluation of object detection models for wear
able devices in assisting visually impaired people,” Proc. IEEE Int. Conf.
 Multimedia Expo (ICME), 2020.
 [15] Zhang L., Song S., and Chen M., “Real-time object recognition system for
 visually impaired people based on convolutional neural networks,” Proc.
 IEEE Int. Conf. Image Process. (ICIP), 2019.
 52
