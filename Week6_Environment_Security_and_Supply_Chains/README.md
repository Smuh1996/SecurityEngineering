
# Secure Running Environment?

It is important to understand the differences and security capabilities of the concepts listed below. Choose two out of the four concepts and write a short explanation of them and their respective security capabilities and incapabilities.

Focus on giving a good overview of the security limits for the concepts.

- TPM
- Enclave
- Container
- Virtualization

**Max 300 words excluding sources.**

#Answer
We will explain two of the following 
1:Enclave 
2: Containers 

Enclave

A security enclave is a secured region within a processor where code as well as data can be stored in a protected way. It helps us to ensure that computations which are very sensitive and  can be performed with varying degrees of isolation from interference by other software or the operating system. This makes them suitable for using them in activities such as protection of sensitive data while the data is under processing.


On other hand enclaves have their security constraints that make them deficient. They depend on the physical foundation.However if there can some errors  in the code written for the enclave then an attacker can attack easily and breach the security that is expected from them.

Containers


Containers are light weight mobile entities that gather applications and their dependencies into one place. They are efficient for deploying applications since they are implemented in the host operating system’s kernel but operate in different user spaces.

However containers have their drawbacks. Because all the containers are based on the same kernel if a hacker finds a way to enter on of the kernel he will be able to access all the containers on the host.


### Task 2: Supply Chain Attacks



Securing the Supply Chain Against Attacks


The supply chain for our company includes a few  key actors:
First of all 
Our company 

That manufactures routers and software.
The second will be Supply components or part suppliers that supply like chips and circuit boards.Transport that manages logistics and delivery of parts and products.And the last one is 
Retail Companies

That sell the products to businesses and consumers.

There are a few thin to keep in mind 

Outsourced Manufacturing: 
Outsourcing of manufacturing of components may present a risk of having the modified by some mischievous individuals. The blamed facilities are not secure enough or not enough overseen, which means that insecure parts could be integrated into end products.

2. Transportation Companies: In shipping, some goods may be seized and changed by other people or organizations. Presence of vulnerable link in the kernel can cause some type of unauthorized access.

3. Retail Companies:If the retail environment is not safe,some products can be tampered with before getting to the consumers. This is dangerous because it translates to passing compromised devices in the market.

4. In-house Employees: The insiders are often a real threat when people have access to some information or applications in the organization. Employee training also becomes a potential security risk when done poorly.

Concrete Actions
Measures for the protection of supply chains
1. Vetting Suppliers
   
Our first step in addressing security of the supply chain should involve conducting stringent supplier certification and Supplier security audit. This step helps to try and eliminate bad components from getting into our supply chain even if it will take some time for production as a result of management taking time to inspect each one.

2. Secure Transportation

Next is security during transit can be improved
through using sealed security bags which can
be sealed in a way that is noticeable if the seal
has been broken, and by having the parcels
GPS tracked. Setting sensitive rules for logistic
individuals assures security and the possibility
to identify any alteration. However this leads to
improvement in the safety of the product it
also implies the incurring of extra costs that
may also lead to a delay in the shipment.

3. Deploy Network Detection and Response 

To prevent any penetration or remain undetected we should use NDR systems in the development and manufacturing of networks. This is useful to us because it allows us to act before such threats materialise. But to be effective it does need continuous investment in technology and people development.

4. Develop User Behavioral Analytics (UBA)

Incorporation of UBA tools will enable us understand the activities of the employees and detect any suspicious activity. If we are able to identify these anomalies.We are able to counter insider threats before they worsen. The drawback is it might increase such privacy issues.

5. Firmware and software update checks demographically

Third-party firmware and software must be audited at least once in a while to determine if there are any vulnerabilities, or malicious codes added in them. This means that only secure update are used to ensure that out final products are not compromised. But these audits have to be carried out independently and may ultimately slow down our updates.

Conclusion

 Protection of our supply chain from attacks include robust supplier verification process, transport security as well as implementing newer technologies such as NDR and UBA. Even though such measures may be a bit resource-demanding and phrase-consuming, the advantages of preserving our products and customers’ confidence are far beyond those challenges. Therefore by trying to identify the possible areas of threats we are capable of protecting ourselves and our clients from supply chain attacks.

---

### Task 3: Securing Docker

**Linux required for full completion; [Course provided VM](https://ouspg.org/archlinux)**

In this exercise we are checking out some tools and practices to help you create better and more secure Docker containers. You are to either use your own Dockerfiles or images, create your own dockerfile for this exercise or you can use ones created by other people. The important part here is auditing and fixing the files, image or container. You shouldn't use ones that have been well audited; the files you choose for this task should provide some output, this is likely with most files.

> We have added an example Dockerfile with an additional file it needs, you may use this. If you are well versed with docker and/or containers in general it might not be the easiest or best way to complete the task, you should build your own file for this task or contribute to open source projects with docker containers. You **need** to download and add permissions for the executable 'docker-entrypoint.sh' file before building.

These tasks provide a great chance to contribute to open source projects, especially if you are looking for a great way to make your first pull requests. You can find Open Source Software with Dockerfiles and lint these, fix the problems provided by the linter when valid, open up a pull request and suggest these fixes with good explanations. 

Your analysis with Trivy (or scanner of your choice) can be opened as an issue, or you can write it into a report and try to open a pull request for it or fixes you made. These might require more work to get accepted though, but can be a great contribution to certain projects.

> A small warning, as some of these tools can be quite complicated, reading through the documentation could take some time. All necessary parts **should** be in this task sheet, but not all problems can be covered. And due to the nature of the course, we expect students to learn and be able to read and take in documentations.

---

### Task 3A) Linting the Dockerfile 0.5p

We will start by first linting the Dockerfile, this will let you know of problems with the configuration, for example using the ```:latest``` tag. These tools will guide you towards  the best practices regarding [Dockerfiles](https://docs.docker.com/develop/develop-images/dockerfile_best-practices/). 

You are free to use any Dockerfile linting tool you want, however a great tool worthy of a recommendation is [Hadolint](https://github.com/hadolint/hadolint), they have the tool packaged into a container and they also have a [GUI Web tool](https://hadolint.github.io/hadolint/) for those interested. The web tool is quite great, but doesn't offer the same customizability as the CLI tool, the functionality is enough for this task, especially if you don't feel comfortable on the command line. As stated, the tool can also be run on Docker, this makes it easier to run on different environments. 

```docker pull hadolint/hadolint```  
To pull the image and can be run with:  
```docker run --rm -i hadolint/hadolint < Dockerfile```

> For running with custom rules and/or personal modifications you should refer to their own [instructions](https://github.com/hadolint/hadolint#how-to-use). 

Depending on the type of Dockerfile you are linting and which tool you are using to do this, you will be presented either with just the problems or the tool can give you directions on fixing these issues. 

Not all problems indicated by the tool have to be fixed, and not all warnings should be fixed blindly, but of course you should aim for fixing everything you can, while not breaking the program.

### What to return:
- What linter you used
- The dockerfile, before and after fixes
- Screenshot **or** .md file of the linter before and after fixes

[Hadolint](https://github.com/hadolint/hadolint)  
[Hadolint Web GUI](https://hadolint.github.io/hadolint/) 

---

### Task 3B) Container Image Analysis 0.5p

Next comes analyzing the image for vulnerabilities in containers. It is also common to use these scanners in CI/CD pipelines. Again, you can use any analyzer you want, but we're going to recommend [Trivy](https://github.com/aquasecurity/trivy). Trivy is an open source project by [Aquasecurity](https://www.aquasec.com/), and it has quite the nice [documentation](https://aquasecurity.github.io/trivy/v0.41/). This task should be doable without reading too much documentation, we do  however recommend checking it out.  They cover at least **most common** use cases and problems there. You can also refer to this documentation if you want to know more about the tool itself and other ways you can use it, such as Kubernetes, filesystem and GitHub repository scanning.

For building from a file named 'Dockerfile' ```docker build -t <name> .```

Trivy can be run on docker or it can be installed from a [binary](https://github.com/aquasecurity/trivy/releases/tag/v0.45.1) or from a [package manager](https://aquasecurity.github.io/trivy/v0.45/getting-started/installation/)  

For Archlinux ```pacman -S trivy```  
And then you can run it with:  
```trivy image <image_name>``` for Docker images.  

Running on docker should work with ```docker run aquasec/trivy image <image_name>```
  
Here you should **try** to fix atleast some errors, the recommended tool Trivy can tell you if a vulnerable piece of software has a patch or a newer version that addressed the vulnerability. However we do understand that not every vulnerability can be fixed.

### What to return:
- What analyzer you used
- The image used, **or** the Dockerfile to build it
- Screenshot **or** .md file of the analyzer output before and after the fixes

[Trivy](https://github.com/aquasecurity/trivy)  
[Trivy docs](https://aquasecurity.github.io/trivy/v0.41/)

---

### Task 3C) Runtime Security 1p

Finally we are going to look at the runtime security of containers, here again you can use any tool you want to, but we're going to recommend a tool originally by [Sysdig](https://sysdig.com/), currently under [CNCF](https://www.cncf.io/). The tool [Falco](https://github.com/falcosecurity/falco) is designed to detect and alert in real-time. The tool is for Linux operating systems.

They as well have a vast and very detailed [documentation](https://falco.org/docs/) with multiple ways to install and run the tool. The documentation has instructions for [installing on different Linux distributions](https://falco.org/docs/getting-started/source/), installing the [falco binary](https://falco.org/docs/getting-started/installation/#falco-binary), and running with Docker, which we recommend here. You can also use their own [tutorials](https://falco.org/docs/tutorials/) to get more familiar with the tool.

### Installing into Docker

For this task we are going to use the Fully Privileged Modern eBPF version, you can find more information and other ways to run it [here](https://falco.org/docs/setup/container/). 

The command provided on the page is  
```
docker pull falcosecurity/falco-no-driver:latest
docker run --rm -it \
           --privileged \
           -v /var/run/docker.sock:/host/var/run/docker.sock \
           -v /proc:/host/proc:ro \
           -v /etc:/host/etc:ro \
           falcosecurity/falco-no-driver:latest
```

This command will be enough to get you up and running with Falco, given you are already using linux with docker working.

### Triggering Alerts

If you used another way to install you need to choose the rules. If you used the method above, you can go forward and start looking at triggering alerts. 

For the task you need to trigger alerts about and from within the containers. One easy way you can trigger an alert is with ```--privileged``` containers, as the ```--privileged``` flag itself creates an alert.  

However you are to trigger another alert from within the containers, here again their documentation provides great instructions on which types of activities create which types of alerts, and with which rulesets, the above method uses the modern eBPF. 

If you are using the example Dockerfile for these tasks, you may for example install and/or run software inside a container for some output from falco.

> `docker run -it <image_name> /bin/sh` can be used to start an interactive shell in a container. You can use any shell you want, like bash, but not every distribution, or container has it.

You can modify the rules provided with the installation, not mandatory, however it is encouraged to take look at least.

### What to return:
- What runtime security scanner you used
- The image used, **or** the Dockerfile to build it
- Screenshot **or** .md file of the alerts created
- What commands and/or activities used to trigger the alerts

[Falco](https://github.com/falcosecurity/falco)  
[Falco docs](https://falco.org/docs/)
