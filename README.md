ABSTRACT 
Telemedicine is an emerging service through which professionals treat the patient using telecommunication technology. Professionals need to access the electronic medical record (EMR) of the patients which can contain huge data. All the healthcare data of the patients which include x-rays, images etc. are private. Due to the large amount of data, it is stored in the cloud. Though cloud is really popular but it has its own security issues. For instance, data theft attacks are the most popular among them. In our project, the main focus is on securing the healthcare cloud data using fog computing to create decoy data. Decoy is used to secure the data stored over cloud. An authentication protocol has been implemented among the three parties based on bilinear pairing cryptography. Using this protocol a secret key is generated and all the parties can communicate securely.  access data effectively. As the patient moves from one hospital to another, cloud can track and manage all those medical records. 
Healthcare cloud has different security issues [2] and handling them is a big challenge because the private information about the patients is stored over cloud. Private medical data of patients need to be secured over cloud in such a way that the process is transparent to them. Different types of attacks are done over cloud to steal the personal information so a proper technique is required to secure cloud computing. 
In our project, we propose a model to secure healthcare data using two main concepts: fog computing and decoy technique. With the help of decoy, a fake set of data is created. It attracts the attackers towards it because looks exactly same as the original one. In other methods, each time an attacker is detected to access the data, decoy is called but in our model decoy data is retrieved first, every time the data is accessed. This method ensures better security and to double this security, the files are encrypted before storing them over cloud. By doing this our technique fully secure the medical data. There is no need to worry if the user is an attacker because he will first access the decoy and the only the legitimate user can access the original data after successful verification. 
Some of the terms related to our proposed work are as follows: 
1.1.  CLOUD COMPUTING 
Cloud computing provides the platform to store, compute and process the data. It is divided mainly into three service models: (a)IaaS, which provides infrastructure for users (b)PaaS, 
3 
 
which provides access to operating system and other services to develop (c)SaaS, which provides access to software applications without installing them on computers and give this service through the internet. Cloud computing can be deployed in three ways: public, private and hybrid cloud. Hybrid cloud has the properties of two or more deployment models. [3]  
Cloud computing has various advantages like: 
1). It is adaptable: Cloud computing provides adaptable programs and applications. 
2). It is multitenant: Cloud computing provides personalized applications to a number of tenants). It is reliable: Cloud computing is very reliable because it is hosted by a third party and if an error will occur, it is easy to access for a customer. 
4). It is scalable: Cloud applications can function across every device and integrate with other applications. 
5). It is secure: Due to increased security and centralization of data cloud computing becomes more secured. 
1.2.  FOG COMPUTING 
Fog computing provides the platform for storage, processing and communication. It is just like cloud computing but it extends cloud computing to the edge of the network [4]. Using this, data can take more advantage of the power of the cloud. The main task of fog computing is to place the data nearer to the user. Creating decoy data and placing it in front of the real information in the cloud to distract attacker is also called as fog computing. Basically, a ‘fog’ of false information is created to protect the user’s real information from attacks. 
When an attacker is detected to access the system, decoy data like decoy files, honey pots can be generated to attract him so that he thinks that he accessed the real data but actually he has not. This decoy and other false information can be created manually but it will be very hectic especially for large organizations which hold huge amount of data that is why fog computing is used to create the decoys. [5] 
4 
 
1.3.  DECOY  
This technique is adapted to decrease the value of information accessed by attackers by giving them false information in place of real. It can be possible only if the decoy has following features: 
1). It should be believable: Decoy should seem so real that the attacker would believe that he has accessed the real and right data. If it does not contain the similar but bogus information then it will not be trustworthy. 
2). It should be attractive: Decoy should be attractive enough to draw attention of the attacker towards it. 
3). It should be perceptible: This is similar as being attractive whereas it is more related to be easily accessible by attackers. In other words, we can say that decoy should be placed in such a place so that attacker can easily track it. 
4). It should be distinguishable: Decoy should be different from the real file so that legitimate user can differentiate between them though it is really difficult to maintain balance between believability and differentiability.  
5). It should not interfere with real files: It is mandatory for a decoy to be non-interfering so that the user would not misuse the bogus information. 
6). It should be detectable: The owners of the decoys should be alerted whenever those will be accessed [6]. 
1.4.  BILINEAR PAIRING FUNCTION 
Bilinear pairing is the mapping between cyclic groups. Let G1 and G2 are two additive and GT to be the multiplicative group and all of them are cyclic groups of prime order q. this pairing is defined as:    e : G1 X G2           GT 
This should satisfy the following properties [7], [8]: 
 It should be bilinear. 
5 
 
  e (aP, bQ) = e (P, Q) ab 
, where ⱯP, Q ∈ G1 and Ɐa, b ∈ Z 
 It should be non-degenerate. 
e(P, P) ≠ 1  It should be computable: If an algorithm exists which can efficiently compute e(P, Q) for any P, Q ∈ G1 then the mapping is said to be computable. Some more properties of bilinear pairing are given below:  e(P, ∞) = 1 and e(∞, P) = 1  e(P, -Q) = e(-P, Q) = e(P, Q)-1  e(P, Q) = e(Q, P) 1.5.  DIFFIE-HELLMAN PROBLEM 
In some pairing protocols, the security can be an issue due to some problems which are very difficult to manage [7], [8]: 
1. Computational bilinear Diffie-Hellman problem (CBDH): The problem is to compute  e(P, P)abc  when P; aP, bP, cP ∈ G1 are given. 2. Decision bilinear Diffie-Hellman problem (DBDH): The problem is to decide e(P, P)abc=r when P, aP, bP, cP ∈ G1 and r ∈ GT are given. 
 
1.6.  ELLIPTIC CURVE DIFFIE-HELLMAN This is a key-agreement protocol rather than encryption algorithm. How keys will be generated and exchanged between parties is done by ECDH and we encrypt the files according to the used algorithm. In our project, files are encrypted using Blowfish algorithm. Keys are generated using ECDH and key agreement is done using Diffie-Hellman. The combination of both these concepts is called as Elliptic Curve Diffie-Hellman (ECDH) [7].  In our project, we use Elliptic curve (EC) not the integers because EC improves the efficiency and supports faster operations. Also, it increases the security even when using 
6 
 
smaller key size. EC gives benefit to use smaller prime and achieves same complexity as with integers. 
 
1.7.  OUR CONTRIBUTION The aim of our project is to remove all the security issues in medical cloud data stored in cloud. Two main concepts fog computing and decoy technique are used. Suitable decoy technique is used to secure the medical data. A gallery of fake data or false information is created which depends on fog computing facility and key pairing protocol and called as decoy medical data. This decoy data is similar to original one but contains bogus information. The files are encrypted using Blowfish encryption algorithm before storing them in the cloud. A secret key is also genon securing the healthcare cloud data using fog computing to create decoy data. Decoy is used to secure the data stored over cloud. An authentication protocol has been implemented among the three parties based on bilinear pairing cryptography. Using this protocol a secret key is generated and all the parties can communicate securely.  
 
 
 
 
 
 
 
 
 
 
 
 
 
2 
 
1. INTRODUCTION 
Cloud computing is defined by the NIST (2009) as “a model for enabling ubiquitous, convenient, on-demand network access to a shared pool of configurable computing resources (e.g., networks, servers, storage, applications, and services) that can be rapidly provisioned and released with minimal management effort or service provider interaction”.[1] Nowadays, cloud is becoming very popular because it gives the platform to store all different information from various sources. In the field of telemedicine, it provides the facility to both medical experts and patients who are far from each other, to access data effectively. As the patient moves from one hospital to another, cloud can track and manage all those medical records. 
Healthcare cloud has different security issues [2] and handling them is a big challenge because the private information about the patients is stored over cloud. Private medical data of patients need to be secured over cloud in such a way that the process is transparent to them. Different types of attacks are done over cloud to steal the personal information so a proper technique is required to secure cloud computing. 
In our project, we propose a model to secure healthcare data using two main concepts: fog computing and decoy technique. With the help of decoy, a fake set of data is created. It attracts the attackers towards it because looks exactly same as the original one. In other methods, each time an attacker is detected to access the data, decoy is called but in our model decoy data is retrieved first, every time the data is accessed. This method ensures better security and to double this security, the files are encrypted before storing them over cloud. By doing this our technique fully secure the medical data. There is no need to worry if the user is an attacker because he will first access the decoy and the only the legitimate user can access the original data after successful verification. 
Some of the terms related to our proposed work are as follows: 
1.1.  CLOUD COMPUTING 
Cloud computing provides the platform to store, compute and process the data. It is divided mainly into three service models: (a)IaaS, which provides infrastructure for users (b)PaaS, 
3 
 
which provides access to operating system and other services to develop (c)SaaS, which provides access to software applications without installing them on computers and give this service through the internet. Cloud computing can be deployed in three ways: public, private and hybrid cloud. Hybrid cloud has the properties of two or more deployment models. [3]  
Cloud computing has various advantages like: 
1). It is adaptable: Cloud computing provides adaptable programs and applications. 
2). It is multitenant: Cloud computing provides personalized applications to a number of tenants. 
3). It is reliable: Cloud computing is very reliable because it is hosted by a third party and if an error will occur, it is easy to access for a customer. 
4). It is scalable: Cloud applications can function across every device and integrate with other applications. 
5). It is secure: Due to increased security and centralization of data cloud computing becomes more secured. 
1.2.  FOG COMPUTING 
Fog computing provides the platform for storage, processing and communication. It is just like cloud computing but it extends cloud computing to the edge of the network [4]. Using this, data can take more advantage of the power of the cloud. The main task of fog computing is to place the data nearer to the user. Creating decoy data and placing it in front of the real information in the cloud to distract attacker is also called as fog computing. Basically, a ‘fog’ of false information is created to protect the user’s real information from attacks. 
When an attacker is detected to access the system, decoy data like decoy files, honey pots can be generated to attract him so that he thinks that he accessed the real data but actually he has not. This decoy and other false information can be created manually but it will be very hectic especially for large organizations which hold huge amount of data that is why fog computing is used to create the decoys. [5] 
4 
 
1.3.  DECOY  
This technique is adapted to decrease the value of information accessed by attackers by giving them false information in place of real. It can be possible only if the decoy has following features: 
1). It should be believable: Decoy should seem so real that the attacker would believe that he has accessed the real and right data. If it does not contain the similar but bogus information then it will not be trustworthy. 
2). It should be attractive: Decoy should be attractive enough to draw attention of the attacker towards it. 
3). It should be perceptible: This is similar as being attractive whereas it is more related to be easily accessible by attackers. In other words, we can say that decoy should be placed in such a place so that attacker can easily track it. 
4). It should be distinguishable: Decoy should be different from the real file so that legitimate user can differentiate between them though it is really difficult to maintain balance between believability and differentiability.  
5). It should not interfere with real files: It is mandatory for a decoy to be non-interfering so that the user would not misuse the bogus information. 
6). It should be detectable: The owners of the decoys should be alerted whenever those will be accessed [6]. 
1.4.  BILINEAR PAIRING FUNCTION 
Bilinear pairing is the mapping between cyclic groups. Let G1 and G2 are two additive and GT to be the multiplicative group and all of them are cyclic groups of prime order q. this pairing is defined as:    e : G1 X G2           GT 
This should satisfy the following properties [7], [8]: 
 It should be bilinear. 
5 
 
  e (aP, bQ) = e (P, Q) ab 
, where ⱯP, Q ∈ G1 and Ɐa, b ∈ Z 
 It should be non-degenerate. 
e(P, P) ≠ 1  It should be computable: If an algorithm exists which can efficiently compute e(P, Q) for any P, Q ∈ G1 then the mapping is said to be computable. Some more properties of bilinear pairing are given below:  e(P, ∞) = 1 and e(∞, P) = 1  e(P, -Q) = e(-P, Q) = e(P, Q)-1  e(P, Q) = e(Q, P) 1.5.  DIFFIE-HELLMAN PROBLEM 
In some pairing protocols, the security can be an issue due to some problems which are very difficult to manage [7], [8]: 
1. Computational bilinear Diffie-Hellman problem (CBDH): The problem is to compute  e(P, P)abc  when P; aP, bP, cP ∈ G1 are given. 2. Decision bilinear Diffie-Hellman problem (DBDH): The problem is to decide e(P, P)abc=r when P, aP, bP, cP ∈ G1 and r ∈ GT are given. 
 
1.6.  ELLIPTIC CURVE DIFFIE-HELLMAN This is a key-agreement protocol rather than encryption algorithm. How keys will be generated and exchanged between parties is done by ECDH and we encrypt the files according to the used algorithm. In our project, files are encrypted using Blowfish algorithm. Keys are generated using ECDH and key agreement is done using Diffie-Hellman. The combination of both these concepts is called as Elliptic Curve Diffie-Hellman (ECDH) [7].  In our project, we use Elliptic curve (EC) not the integers because EC improves the efficiency and supports faster operations. Also, it increases the security even when using 
6 
 
smaller key size. EC gives benefit to use smaller prime and achieves same complexity as with integers. 
 
1.7.  OUR CONTRIBUTION The aim of our project is to remove all the security issues in medical cloud data stored in cloud. Two main concepts fog computing and decoy technique are used. Suitable decoy technique is used to secure the medical data. A gallery of fake data or false information is created which depends on fog computing facility and key pairing protocol and called as decoy medical data. This decoy data is similar to original one but contains bogus information. The files are encrypted using Blowfish encryption algorithm before storing them in the cloud. A secret key is also generated for secure communication among all parties by using Pairing based cryptography to access and store data in the cloud. 
 
  
 
 
 
 
 
 
 
 
 
 
  
7 
 
2. MOTIVATION 
Healthcare cloud contains the huge amount of medical data of the patients which is shared by a number of organizations. The doctors can treat their patients remotely and can access their medical EMR, reports, prescriptions etc. even they are not near them. In the process of digitization, all the personal medical data is shared on the internet and are very less secure. The probability of data theft attacks on the medical data stored in cloud is very large. User’s personal information like credit card information, social security numbers, passwords etc. is the main target of the attackers. By 2020, it is predicted that the attacks on medical data will increase four times.  
Electronic medical data is a very easy way to earn wealth. It can be used to claim fraud insurance, obtain prescription medication, theft of advanced identity. Personal medical data is more valuable than credit card information. It is observed that in black market credit card number is sold for $1 whereas a medical image is sold for $50. Credit cards can be replaced if they are stolen but this is not the case with medical data. Even in this situation the health organizations have not invested in creating the robust IT security system that can protect the personal data of patients. 
A study is done on the population of Saudi on the contents of the mobile phones [9]. According to the results, 88% of the females answered “personal photos” and 63% males answered “personal information” and “personal photos”. This study shows that some information can be important to someone and not to other.  So after seeing the huge issue of the security of medical personal data stored in cloud, we propose a model to secure it. In our model, we see the suitability of the already existing decoy technique for protecting the data stored in cloud. 
 
 
 
 
8 
 
3. LITERATURE SURVEY 
Cloud data can be secured in many ways using decoy technique. In this section, various studies are presented. According to Vikas et al. [10], there are several issues in mobile computing. These threads are physical threats, application-based threats, network based threats, web based threats and other active threats.  
There are different situations in which decoy can be implemented to secure cloud data. Voris et al. [11] discussed all these scenarios. Decoy can be placed at a local computer where it is created and on a network. In both situations, decoy is used to protect the real data on different level. Decoy software can save the real software form being stolen. Decoy used in cloud is used to protect the personal data stored in the cloud. Sangle et al. [12] discussed how attacks are prevented using decoy technique given by fog computing. When any attacker is assumed to access the data, a flood of fake/bogus information is returned to the real data to dilute the essence of real data. By observing the data patterns, data attacks can be detected and whenever such situation occurs a huge amount of data is returned to the attacker. In this way, the real data is protected using decoy. 
Khairnar and Borkar [13] explained the method that is used to secure cloud data in the following scenario: when a user logs in to the system, a “Successful login'' SMS is sent to his/her mobile device. The user can execute all tasks after answering the security question. There can be two situations: first the user correctly gives the answer then the real data is downloaded but if he can not give the correct answer then it is confirmed that he is an attacker then the decoy is downloaded. In this situation, the mail/SMS is sent to the owner of the data.   In the referenced literature various techniques and models are introduced to secure the medical data in the cloud. Various hybrid techniques are also given because sometimes, a single security algorithm is not sufficient. In aforementioned papers, the offensive decoy technique is used it means that when there is an attack detected then only the decoy is created but in our project we propose the model in which decoy is accessed at the very first step whether he is user or attacker. This enhances the security level. Also to double the security, the files are encrypted before storing them to the cloud.  
9 
 
4. PRIVACY PRESERVING MODEL TO SECURE MEDICAL CLOUD DATA 
We propose a privacy preserving model to secure patients’ medical data stored in the cloud. Cloud has its own security issues and to protect the personal data stored over it, fog computing and decoy technique are used mainly. Similar as real but bogus information is generated to attract the attacker, this false information is called decoy. To enhance the security files are encrypted before storing them over cloud. Pairing-based cryptography is used to generate the key to establish secure communication among all the parties.    
4.1.  SYSTEM ARCHITECTURE 
The System consists of user, fog node and cloud. The user uploads encrypted medical image to the cloud. A decoy image of the same category is added to the decoy database on the fog node. When user access his account for downloading an image he is first referred to the decoy database irrespective of the fact whether he is a legitimate user or an attacker. By doing this, the security is increased double times. If he is an attacker and tries to download the decoy data by assuming it the real information, a mail is sent to the owner of the data alerting him that his personal data has been accessed. If he is a legitimate user, he can differentiate between his personal information and decoy. So after a successful verification by passing the security question he can access and download his personal medical data.  
The fake galley and the real one are similar to each other when a legitimate user uploads a medical image in the cloud, at the same time a decoy image is uploaded from fog computing to his gallery of decoy data. While uploading the photo on cloud, user needs to recognize the category of it so that the decoy image will be uploaded to the same folder in decoy gallery. This makes the attacker more to believe that he has accessed the real information. In our project, the decoy image is not added manually but automatically. 
 
 
10 
 
 
Fig. 1: System Architecture for proposed model 
4.2.  METHODOLOGY 
In our proposed method, a decoy database is created on fog node using decoy technique to secure medical data over cloud where original data is stored. When user registers with the service a shared secret key is generated for user, original database and decoy database using pairing based cryptography. When user uploads an image to his account, the image is first encrypted using the secret key generated during registration and is then stored over the cloud. A decoy medical image of the same category as the uploaded image (like MRI, X-RAY, etc) is added to decoy database in parallel.  
When a user accesses his account, he is first referred to decoy data irrespective of whether he is a legitimate user or an attacker. An attacker will believe that he has accessed the original 
11 
 
data and will download the decoy medical images. When an attacker downloads decoy data, an email is sent to user warning him that someone has tried to access his account.  
A legitimate user will recognize decoy data and thus will move to next step. In the second step, a legitimate user is verified using a security question. If verification turns to be true, he is referred to original medical data. When user downloads an image from original database, the image first decrypted using the same secret key as was used during encryption and is then downloaded over users system.  
The communication between the user, original database and decoy database is made secure using the secret key shared between the three parties during registration. An authentication protocol is implemented that uses the shared secret key and parties’ public identity to authenticate them during communication and allow exchange of messages between them. 
 
4.3.  CREATING DECOY MEDICAL DATA 
Decoy medical data is not directly useful to the legitimate users but it protects the patients’ real medical data by distracting the attacker from it and attracting towards the decoy data. The cloud contains the decoy medical data which is placed in fog computing near original data. Fog computing provides the facility of decoy file system. Every time the user uploads a new medical image in his gallery, a decoy image is uploaded to the decoy gallery at the same time. This process of adding a decoy image for every new image is done automatically not manually. 
4.4.  KEY EXCHANGE ALGORITHM 
The user, original database and decoy database communicates with each other in different scenarios. For example, to upload an image user sends original encrypted image to the cloud, the cloud stores the image and then asks decoy database to add a decoy image in parallel. The communication between user, original database and decoy medical data is made secure using pairing based cryptography. The Elliptic curve cryptography is used to generate keys and Diffie-Hellman is used for key agreement.  
12 
 
Whenever a user registers with the service, the key generator determines following parameters: 
 Two groups one additive, G1 and other multiplicative, G2 of the same prime order q.  A generator P of G1.  A bilinear map e: G1 X G2         G2 
 
4.4.1. KEY GENERATION Key Generator selects k+1 random numbers (r0, r1… rk) ∈ Zq* and generates a polynomial g(x) = r0x0 + r1x1 + ……. + rkxk. Key generator also computes g(id) = r0(id)0 + r1(id)1 + …… + rk(id)k where id  ∈ Zq* corresponding to the identity of each user, original database and decoy database. The identities of user, original database and decoy database acts as their public keys. The parties send their public keys to the key generator and receive their corresponding private keys computed by the generator through a secure channel. The public and private keys are represented as:  For user: Public Key: idu  and Private Key: Vu = g(idu)  For original database: Public Key: ido  and Private Key: Vo  = g(ido)  For decoy database: Public Key: idd  and Private Key: Vd  = g(idd) 
 
 
4.4.2. KEY AGREEMENT Using parameters determined by key generator the three parties: user, original database and decoy database computes a shared secret key. Firstly, user computes Yu = VuP and sends it to original database and decoy database. Similarly, original database computes and decoy database computes Yc = VcP and Yd = VdP respectively and then, sends them to other two parties. From the received values, all the three parties compute their secret key:  User: Su = e(Yc, Yd)Vu  = e(P,P)VuVoVd  Original Database: So = e(Yu, Yd)Vo  = e(P,P)VuVoVd  Decoy Database: Sd = e(Yu, Yo)Vd  = e(P,P)VuVoVd 
 
13 
 
4.4.3. AUTHENTICATION PROTOCOL 
Now, to communicate and exchange messages, parties must authenticate each other. The secret key computed in previous steps is used by the parties to authenticate each other during any communication. Each party encrypts the public key of the receiver with the shared secret key and sends the encrypted value along with the messages to the receiver. Receiving party decrypts the encrypted value using the same secret key to confirm that the message has been sent by the legitimate party.   
  
4.5.  PHOTO ENCRYPTION ALGORITHM 
Photo encryption is a method to make a photo secure by converting into an understandable form. There are various types of photo encryption algorithms. Different encryption algorithm has different level of security and different properties. In our project, we are using Blowfish Encryption algorithm. Blowfish is a symmetric key algorithm where key is not changed. This algorithm has its own advantages. We choose this algorithm due to the following reasons: 
1. It is the most secure algorithm of all because it has the longer key length. 2. Photo of any format, any color whether it is black and white or colored, can be encrypted using Blowfish algorithm. 
The photo is encrypted using the secret key generated by public key generator (PKG), used for establishing secure communication among participating parties. After that, photo is encrypted according to process of Blowfish. First of all, there is the division of the photo in the form of a matrix. Only the header of the photo is not encrypted but the whole image. These elements of the matrix are stored row-wise in the photo from left to right. Photo rows are encrypted from top to bottom. 
 
 
 
14 
 
4.6.  PHOTO DECRYPTION ALGORITHM 
The task of the photo decryption algorithm is totally reverse of the photo encryption. Using photo decryption, the encrypted photo is converted back to the original one. The key is used as same for the encryption. The sub-keys are supplied in reverse order in the decryption process. This is the only difference between encryption and decryption. 
 
           
  Cipher Image 
 
key 
 
   
key 
                                               Fig. 2: Encryption and Decryption Model 
Above figure shows the process of encryption and decryption. To encrypt a photo the required inputs are plain medical image and a key. The photo is converted to the cipher image which is not understandable to the one who has not the key to decrypt it again. Now here comes the decryption process. For this, the required inputs are the encrypted photo/cipher image and the same key used for encryption. The photo is converted to the original one, which is plain medical image. 
 
 
 
Plain Medical Image 
 Photo Encryption Model 
Plain Medical Image  Photo Decryption Model 
15 
 
4.7.  ACCESSING ORIGINAL MEDICAL DATA 
Original medical data contains user’s real data which are being secured by our model. This real information is stored in the cloud. At the very first step, verification is done by passing the security question only then the legitimate user can access his personal data. When user uploads the original image, a decoy image is also uploaded to decoy gallery in parallel. The original image is encrypted before storing it before cloud. 
Our model proposes double level of security: 
1. Decoy technique in which fog of misinformation is created to distract the attacker. 2. The photo is encrypted before storing it in the cloud. 
So, we can say that our model enhances the security by using both encryption and concept of decoy gallery created with the help of fog computing. 
 
4.8.  IMPLEMENTATION DETAILS 
This project is made in php using AWS cloud and wamp server. Java language is used for encryption and key pair generation. Two systems are connected; one act as user and other acts as fog node. The original images are encrypted and stored in cloud database, at the same time decoy images are created at fog node and stored in fog database at wamp server. When user request for download, it will first go to fog node where decoy data is present and then he/she will pass the security question and download the original image. 
 
 
 
 
 
16 
 
5. DATA FLOW DIAGRAMS 5.1.  LEVEL 0 
 
 
 
 
 
      Fig. 3: Level 0 Data Flow Diagram 
 
 
 
 
 
 
17 
 
5.2.  LEVEL 1 
   
 
 
            
 Fig. 4: Level 1 Data Flow Diagram for uploading an image 
 
 
 
 
 
18 
 
 
 
          
                 Fig. 5: Level 1 Data Flow Diagram for user to download an image  
 
 
                                      Fig. 6: Level 1 Data Flow Diagram for attacker 
 
19 
 
5.3.  LEVEL 2 
 
 
   Fig. 7: Level 2 Data Flow Diagram to upload an image 
 
 
20 
 
 
  
 
                         Fig. 8: Level Data Flow Diagram for user to download an image  
 
 
 
 
 
 
  
 
21 
 
 
 
 
Fig.9: Level 2 Data Flow Diagram for attacker 
 
 
 
22 
 
6. RESULTS 
In our proposed scheme, pairing based elliptic curve cryptography is used to secure communication. Cryptographic computation involves one elliptic point multiplication, one elliptic point addition operation, two modular multiplication and one modular addition operation. As compared to existing scheme, our scheme involves lesser number of operations and thus has lower computational cost. 
 
Fig. 10: Comparison Graph between Hwang Scheme and our proposed Scheme 
7. CONCLUSION AND FUTURE PLAN 
We propose a privacy preserving model to secure medical data stored over cloud using fog computing and pairing based cryptography. Decoy technique is used to hide original medical data by creating a decoy database on fog node. When user accesses his account he is referred to decoy database which prevents original database from any inside attack. The original database is accessible only to user after verification against a security question. To improve security, an authentication protocol has been proposed among user, original database and decoy database using pairing based cryptography. 
In future, we plan to implement user profiling at fog node to detect any unusual data access patterns to further increase security against insider malicious attacks.   erated for secure communication among all parties by using Pairing based cryptography to access and store data in the cloud. 
