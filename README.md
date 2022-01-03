# GitlabUpdate
This is the small guide to upgrade your Gitlab Community Edition from &lt; 12.10.14 to > 14.2.6

# To upgrade your instance please follow the below steps.

1. Access you ubuntu machine (I used AWS Ec2 instance) and make sure machine must have some extra space inn root directory.
2. To upgrade you must need to follow the version path (https://docs.gitlab.com/ee/update/#upgrade-paths)
3. Check your curent gitlab version by using **sudo gitlab-rake gitlab:env:info**
4. Now you need to upgrade your ubuntu package manager **sudo apt-get update**
5. **sudo apt-get install gitlab-ce=13.0.14-ce.0**
6. **sudo apt-get install gitlab-ce=13.0.14-ce.0**
7. **sudo apt-get install gitlab-ce=13.1.11-ce.0**
8. **sudo apt-get install gitlab-ce=13.8.8-ce.0**
9. **sudo apt-get install gitlab-ce=13.12.10-ce.0**
10.**sudo apt-get install gitlab-ce=13.12.12-ce.0**
11. After this you need to change the gitlab config file, Go to **cd /etc/gitlab/gitlab.rb**
12. Search for unicorn and disable all line using leading # and change puma to true and change puma['port'] = 9999
13. **sudo apt-get install gitlab-ce=14.0.11-ce.0**
14. **sudo apt-get install gitlab-ce=14.1.8-ce.0**
15. **sudo apt-get install gitlab-ce=14.2.6-ce.0**

**Updated**
