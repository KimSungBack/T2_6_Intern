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



hello_t2.py URI
<pre><code>s3://superman-kim-bucket01/hello_t2.py
</code></pre>
