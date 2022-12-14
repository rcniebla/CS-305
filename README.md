# CS-305
CS-305 Software Security

*Briefly summarize your client, Artemis Financial, and their software requirements. Who was the client? What issue did they want you to address?
  Artemis Financial is a consulting company that created financial plans for various clients.  They requested assistance with modernizing their application and implementing industry standard security practices.

*What did you do very well when you found your client’s software security vulnerabilities? Why is it important to code securely? What value does software security add to a company’s overall wellbeing?
  I feel I was able to adequately address all the security concerns that were raised by Artemis Financial for the sake of the exercise but feel that a real application with more than a few classes would need significantly more resources and a longer time period to adapt changes. It is important to code securely because it is one of your jobs as developer to safeguard the information that has been entrusted to you. The consequences for a data breach are significant for companies and customers alike, so it is everyone best interest to code as securely as is reasonable. 

*What part of the vulnerability assessment was challenging or helpful to you?
  Creating the cipher was a bit challenging at first as I had no experience with the libraries but pretty straight forward after I figured them out. I am a firm believer in experimentation and reputation as being great teachers so this opened to door to try to implement different ciphers.  Overall the whole project was very helpful and there is a lot I can use going forward.

*How did you increase layers of security? In the future, what would you use to assess vulnerabilities and decide which mitigation techniques to use?
  I increased security mainly by updating the versions of different dependencies and implementing the cipher.  Going forward I would try to implement a FOSS scan in a Jenkins pipeline to test all the dependencies every time this is run to make sure we are addressing security concerns.  The other thing is implementing a linter to take use of while coding helps prevent bad practices as well as a peer code review before pushing anything to a master branch. 

*How did you make certain the code and software application were functional and secure? After refactoring the code, how did you check to see whether you introduced new vulnerabilities?
  I linted the code and did a manual review myself.  I tested the cipher with multiple inputs to confirm the same string for the same input as well as ran the dependencies check.  To check for new vulnerabilities I ran the dependencies check again and after I increased the version of spring boot ran it again to confirm I wasn’t adding any other issues.  We still saw an issue with snakeyaml but that has not been addressed thus far so I suppressed it for the time being.  In a real project this would need to be made a backlog item to be reevaluated periodically.

*What resources, tools, or coding practices did you use that might be helpful in future assignments or tasks?
  I tried to use best practices when coding.  I implemented a linter to help catch code smells and I addressed the ones that I created. I testing iteratively through the process to make sure the code was functioning like is should and saved the dependency test results in the target folder to validate my progress

*Employers sometimes ask for examples of work that you have successfully completed to show your skills, knowledge, and experience. What might you show future employers from this assignment?
  I would show the implementation of the hashing function and would show the dependency reports along with the process that I took to solve some of the issues that we have found.  As a developer I know how valuable it is to be able to address FOSS findings and I believe that would be a great thing to show an employer.
