1. In your own words describe 3 types of security testing and give an example of each?
	1. SAST - static application security testing: Scans code before it is complied. Takes place early in the SDLC before code is committed. An example is running a security scan on my password.py with Bandit Python Module before I commit my code in Github. (done during unit testing??)
	2. DAST - Dynamic Application Security Testing: Communicates through a website's front end to identify potential security vulnerabilities. Is done once code is live in production on a company's website (done during functional testing??)
	3. IAST - Interactive Application Security Testing: analyzes code for security vulnerabilities during automated QA testing. (done during integration testing???)
2. Is dependency management more or less important than security testings? Why or why not?
	I think dependency management is more important than security testing. For example if your website has a dependency on Adobe for it's images and you haven't properly managed that dependency, all of your website images could disappear if there's a change that's unmanaged to the adobe code. However, if you're website gets hacked because you have a vulnerability and it's down for hours due to a DNS attack, you could easily loose millions in revenue.
3. How does a dependency manager work? Why would we need one?
	A dependency manager works by working closely with software repositories (github, circle ci) and app stores. They can identify and resolve dependencies before code is deployed into production. They coordinate the integration of external libraries or packages into a larger application stack.
	We need one if our code depends on other libraries or applications. 
4. What are the 3 most important steps on the path to production?
	1. Build artifact - code!
	2. Deploy
Monitor?? - Security ![image](https://user-images.githubusercontent.com/80227752/113218592-ccbce280-924d-11eb-9f89-c92ce5a09f90.png)
