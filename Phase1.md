## Phase1

#### 1.bastion -> WAS접속
<pre><code>ssh -i "superman-kim-T2-Internship.pem" ec2-user@10.40.2.78
</code></pre>
#### 2.bastion -> WEB접속
<pre><code>ssh -i "superman-kim-T2-Internship.pem" ec2-user@10.40.2.100
</code></pre>
#### 3.WAS -> OnPremise WEB접속
<pre><code>ssh -i "superman-kim-T2-Internship.pem" ec2-user@192.168.3.164
</code></pre>
#### S3 URI
<pre><code>aws s3 cp s3://superman-kim-bucket01/hello_t2.py hello_t2.py
aws s3 cp s3://superman-kim-bucket01/superman-kim-T2-Internship.pem superman-kim-T2-Internship.pem
</code></pre>
#### zzzz

<pre><code>keypair복사 
aws s3 cp s3://superman-kim-bucket01/superman-kim-T2-Internship.pem superman-kim-T2-Internship.pem
chmod 400 superman-kim-T2-Internship.pem

ssh -i "superman-kim-T2-Internship.pem" ec2-user@10.40.0.94
--> bastion 접속
ssh -i "superman-kim-T2-Internship.pem" ec2-user@10.40.2.78
--> web접속
ping 192.168.3.164

ssh -i "superman-kim-T2-Internship.pem" ec2-user@192.168.3.164
--> op web접속
 
 
ssh -i "superman-kim-T2-Internship.pem" ec2-user@10.40.2.100
--> WAS1접속

ssh -i "superman-kim-T2-Internship.pem" ec2-user@10.40.3.172
--> WAS2접속
</code></pre>
