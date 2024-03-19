# Launch-an-EC2-Instance
## Below are the steps to launch an EC2 instance with a Linux AMI and succesfully ssh into it.

1.	Log into your console and search for EC2 on the search bar (Red Arrow) and click on Launch Instance button (Black Arrow)
    ![Launch EC2](https://github.com/vmk81/Launch-an-EC2-Instance/assets/157844406/06d64b20-40ba-43df-82bf-303dfc731327)
  	
2.	On the ‘Launch an Instance’ page use the following parameters   
Name = EC2-Docker  
AMI = Amazon Linux  
Instance Type = t2.micro  
Key pair = EC2Docker (and then click create new key pair and download the pair to your desktop)  

3.	After the above is done under Inbound Security Group rules click on ‘Add a Security group rule’ button (Red Arrow). Under Type select HTTP (Black Arrow) and source type Anywhere (Yellow Arrow). Then click Launch Instance button (Blue Arrow) 
   ![Inbound Security Group](https://github.com/vmk81/Launch-an-EC2-Instance/assets/157844406/cb34f64c-e120-4c3c-a66a-db97ca24bbc6)

4.	Once your Instance is launched go back to your Instances page and you should see your EC2 instance running (Red Arrow). Select your Instance and click on Connect button (Black Arrow) to log into your Instance. 
   ![Connect to EC2](https://github.com/vmk81/Launch-an-EC2-Instance/assets/157844406/475fe885-fb8f-415b-bdf4-2010168e000f)

5.	On the Connect to instance page select EC2 Instance Connect (Red Arrow) and click on Connect(Black Arrow)
    ![Connect to EC2-2](https://github.com/vmk81/Launch-an-EC2-Instance/assets/157844406/6661bb6e-6018-4f63-a03e-7c4e8dc06935)

6.	After you connect to the EC2 instance you should be able to see the below screen
    ![EC2-Shell Prompt](https://github.com/vmk81/Launch-an-EC2-Instance/assets/157844406/657f10d7-b6f3-445b-b523-5dd09701854a)

7.	On your desktop, open a power shell prompt and navigate to the folder where the keypair was downloaded from step 2. Then type the ssh command using the key pair like in the screenshot below. This will let you log into the EC2 instance using ssh.  
    ![12-ssh](https://github.com/vmk81/Launch-an-EC2-Instance/assets/157844406/e2753bb1-50f9-46f2-8777-33410665e73a)


        
