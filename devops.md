# DevOps

## Version Control
- [Git](https://git-scm.com/) - Best, most ubiquitous version control technology in the world, to the best of my knowledge. It was developed by Linus Torvalds himself to manage Linux core contributions in the late 90's. 
- [Fossil SCM](https://fossil-scm.org/index.html/doc/trunk/www/index.wiki) - a new-ish contender to Git which is fairly compelling for a variety of technological and workflow reasons. Something to watch. But, for now, stick with Git.
- A nice [Git Tutorial](https://try.github.io/levels/1/challenges/1) from Github.
- [GitHub](https://github.com) - Amazing universe of open-source software. Unlimited hosting of open-source repositories. Has issue, milestone, and project tracking. Has project wikis. Integrates with everything.
- [Bitbucket](https://bitbucket.org) - Like GitHub, but unlimited hosting for **private** repositories, which can be nice for internal or sensitive State projects. Also has wikis and its own CI/CD technology called Pipelines built-in. Before it was cancelled as a project by someone to remain nameless, ODE was going to convert all existing Version Control systems in the State (of which there are nine, costing over $100,000 annually) to Git/Bitbucket Enterprise. Someday...
- [CodeGiant](https://codegiant.io/home) - New entrant hoping to offer a better-designed experience. 

### Git Clients

- [GitHub Desktop](https://desktop.github.com/) - simple, nice-looking, approachable client. 
- [SourceTree](https://www.sourcetreeapp.com/) - from Atlassian, makers of Bitbucket.
- [GitKraken](https://www.gitkraken.com) - beautifully designed Git Client.
- [Original Git Bash Shell](https://git-scm.com/downloads) - for ballers. This actually comes with GitHub Desktop and SourceTree, so usually doesn't have to be downloaded separately. 

## Containers

- [Vagrant](http://www.vagrantup.com) - easy to spin up virtual machines, configurable via simple YAML files.
- [Docker](https://www.docker.com) - **THE** base container technology. Easy to configure, stitch together, and lock down. Preferable these days to Vagrant.
    + This is the official Docker tutorial. 
    + [Just enough Docker to be Dangerous](http://seankross.com/2017/09/17/Enough-Docker-to-be-Dangerous.html) is a good intro tutorial, as well, by Sean Kross. 
- [Kubernetes](https://kubernetes.io/) - The industry-standard way to scale out and coordinate tons of Docker images working together. Kind of amazing, really.
- [Scotch Box](https://box.scotch.io/) - Pre-configured Vagrant box. Very nice - everything just spins up and works. 

## Automation Frameworks
 
- [Ansible](https://www.ansible.com/) - SSH-based automation technology.
- [Cisco Shipped](https://ciscoshipped.io/)
- [Mantl](http://mantl.io/)

## Continuous Integration / Continuous Delivery

- [Travis](https://travis-ci.org/)
- [Jenkins](https://jenkins.io/)
- 

## Automated Testing

- [Sauce Labs](https://saucelabs.com/open-source)
- [Go Replay](https://goreplay.org/) - Way to reproduce production traffic against a test instance. 

## Database Deployment Tools

- [Flayway DB](https://flywaydb.org/)

