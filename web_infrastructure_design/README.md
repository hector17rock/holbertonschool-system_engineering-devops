# 🌐 Web Infrastructure Design

This directory contains different web infrastructure designs for hosting www.foobar.com, showing how websites can be built from simple single-server setups to complex scalable architectures. 🚀

## 📁 Files in this directory

### 0-simple_web_stack 🏠
Shows the basics - one server doing everything. This is where most websites start but has some serious problems like being a single point of failure.

**What it has:** 📦
- 1️⃣ server with everything on it
- 🌐 Nginx web server
- 💻 Application code
- 🗃️ MySQL database
- 🔗 Domain pointing to the server

**Good for:** 📚 Learning the basics, very small websites  
**Problems:** ⚠️ If the server goes down, everything stops working

### 1-distributed_web_infrastructure ⚖️
Steps it up with multiple servers and a load balancer. Much more reliable than the simple setup.

**What it has:** 🔧
- ⚖️ Load balancer (HAProxy) to spread traffic around
- 2️⃣ web servers instead of 1
- 🔄 Database replication for backup
- 📈 Better performance and some redundancy

**Good for:** 🎯 Medium websites with decent traffic  
**Problems:** ⚠️ Still some single points of failure, no security features

### 2-secured_and_monitored_web_infrastructure 🔐
Adds proper security and monitoring to the distributed setup. This is getting closer to production-ready.

**What it has:** 🛡️
- 3️⃣ firewalls protecting different parts
- 🔒 HTTPS encryption with SSL certificate  
- 👀 Monitoring tools watching everything
- ⚖️ Same distributed setup as task 1

**Good for:** 🏢 Real websites that need security and monitoring  
**Problems:** ⚠️ Still not perfect - has some architectural issues

### 3-scale_up 📊
Takes the secure setup and makes it even more scalable and reliable by separating concerns.

**What it has:** 🎛️
- 🎯 Separate servers for different jobs
- ⚖️⚖️ Multiple load balancers for redundancy
- 🏗️ Better separation of web, app, and database tiers
- 🚀 Can handle much more traffic

**Good for:** 🌟 Large websites with lots of users  
**Problems:** ⚠️ More complex to manage

## 📈 Learning progression

Each file builds on the previous one:
1. **Simple** 🏠 → Learn the basic components
2. **Distributed** ⚖️ → Add redundancy and load balancing  
3. **Secured** 🔐 → Add security and monitoring
4. **Scaled** 📊 → Separate concerns and improve architecture

## 🔑 Key concepts covered

- **Load balancing:** ⚖️ Spreading traffic across multiple servers
- **Database replication:** 🔄 Keeping backup copies of data
- **Security:** 🛡️ Firewalls and HTTPS encryption
- **Monitoring:** 👀 Keeping track of system health
- **Scaling:** 📈 Making systems handle more users
- **Architecture:** 🏗️ How to organize different components

## 🚨 Common problems addressed

- ❌ Single points of failure
- 🐌 Performance bottlenecks  
- 🔓 Security vulnerabilities
- 🙈 Lack of monitoring
- 📉 Scaling limitations
- ⏰ Maintenance downtime

Each design shows how real websites evolve from simple beginnings to complex, scalable infrastructures that can handle millions of users. 🌍✨

## 👨‍💻 Author

**Héctor Soto**  
🤯 💻🪫 Building the future, one commit at a time!  
GitHub: [@hector17rock](https://github.com/hector17rock)
