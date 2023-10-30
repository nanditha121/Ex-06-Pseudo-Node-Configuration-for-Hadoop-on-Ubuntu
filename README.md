# Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu

## AIM

To implement Pseudo Node configuration for Hadoop on ubuntu

## Pre-requisites

a) jdk

Single-Node Configuration

1.	Create a dedicated user account for hadoop

   ![image](https://github.com/nanditha121/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209508/93facdde-d7fa-4265-b883-d7963fbcf78c)


2.	Install java1.8 in folder /usr/local


 ![image](https://github.com/nanditha121/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209508/c1c3bdfd-eeab-4b0e-889d-4cb001932441)


3.	Install Hadoop


  ![image](https://github.com/nanditha121/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209508/664a61b1-8f97-4b93-ad15-e4f7bf20c641)



4.	Set the hadoop environment variables: Include the following lines in the
$HOME/.bashrc file


 
 ![image](https://github.com/nanditha121/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209508/a907cb77-f9ec-450f-b701-d0cf3eac637f)


5.	Set hadoop environment variables: Include the following lines /etc/profile file


![image](https://github.com/nanditha121/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209508/a3a77597-7d60-4fd8-b451-b8a6860b56b3)



6.	Run the.bashrc & profile files from the $ prompt for updating the changes


![image](https://github.com/nanditha121/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209508/ed3503b4-41e4-4358-b132-279422f0bd28)


$ bin/hadoop version	

7.	Configuration of the hadoop files: hadoop-env.sh, core-site.xml, mapred-site.xml, hdfs- site.xml and yarn-site.xml

path ::	/usr/local/hadoop-2.5.1/etc/hadoop

a)	hadoop-env.sh
Include the following lines in hadoop-env.sh file

![image](https://github.com/nanditha121/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209508/f868119b-b114-4323-8bd7-3cd5328a54e0)


b)	core-site.xml
Configure the directory for Hadoop to store its data files, the network ports it listens to, etc. Setup will use Hadoop’s Distributed File System (HDFS-single local machine)

![image](https://github.com/nanditha121/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209508/34be2333-7b18-4c07-b82e-5117ad5a5514)

 
Include the following lines in core-site.xml file between <configuration> and
</configuration> tags

![image](https://github.com/nanditha121/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209508/d49560f4-3c61-46ec-ac11-4ea5c37c8fbe)


c)	mapred-site.xml
 
 ![image](https://github.com/nanditha121/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209508/7ad832ee-93c4-45f5-b36c-691ef950f3be)


Include the following lines in mapred-site.xml file
 

d)	hdfs-site.xml
Include the following lines in hdfs-site.xml file

![image](https://github.com/nanditha121/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209508/2ae704dd-bb1d-40b3-9415-2273f3f10e04)


e)	yarn-site.xml
Include the following lines in yarn-site.xml file

![image](https://github.com/nanditha121/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209508/9fc69128-7cd2-4320-97ad-8010b188844f)


8.	Format the Hadoop File system implemented on top of the local file system using


  ![image](https://github.com/nanditha121/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209508/109d3a88-7a6e-479c-b405-312bff3bab55)


9.	Start Hadoop using

![image](https://github.com/nanditha121/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209508/5e293b69-e988-44ce-9750-0fdf028b3351)


Explore Hadoop using http://localhost:50070/ from the browser	
 
10.	The commonly used HDFS Commands are as follows:

![image](https://github.com/nanditha121/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209508/2a44249b-31e8-44b3-9b80-1c368a32aaef)



11.	Create a directory ‘/input’ in HDFS

![image](https://github.com/nanditha121/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209508/ec3dea2a-6afc-4185-9db1-ff3b0baac68f)

  
12.	Copy the input files into the distributed file system

![image](https://github.com/nanditha121/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209508/c3e57f0f-d6a1-4559-a12c-621ad01c4a38)



13.	Run some of the examples provided


![image](https://github.com/nanditha121/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209508/d7e23fe9-6d2c-4e5d-98d5-b7a22fda6380)


14.	Examine the output files

    ![image](https://github.com/nanditha121/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209508/3b50cc2f-c520-424c-a628-e3e81c5d3edd)
Copy the output files from the distributed file system to the local file system and examine them:

![image](https://github.com/nanditha121/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209508/297322e1-1695-4b39-9b95-a18268fe8906)


 
or

![image](https://github.com/nanditha121/Ex-06-Pseudo-Node-Configuration-for-Hadoop-on-Ubuntu/assets/142209508/249ef8ef-fd58-4ce9-884a-507422a02788)

View the output files on the distributed file system

## Result:
Thus, the implementation of Pseudo Node configuration for Hadoop on ubuntu is successfully executed.
