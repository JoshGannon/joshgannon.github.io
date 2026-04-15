# Forging high productivity under heavy time constraints

I'll provide a high-level overview of a massive firewall upgrade/roll-out, what made it successful, and what I learned.

Due to vendor hardware upgrades and thousands of firewalls needing this replacement of critical infrastructure, I was tasked with creating a technical, semi-automated approach across multiple teams to meet the deadline.

Task: upgrade firewalls in a highly complex configuration environment. Requirement: increase efficiency by at least 4x. Requirement: Build as custom, from scratch, to ensure stability and high quality. Problem?: Vendor cli syntax was not forward-compatible with their own, new hardware/firmware.

## Finding a way forward

Identified all custom components of these configurations via cli. 

Worked with the Development team to pull these cli configurations across the fleet.

Identified all cli components that weren't forward-compatible and solved for the needed resulting cli.

Added complexity: a new requirement was to maintain configuration customization, even if the boxes were licensed or not. This meant knowing which features could be pushed pre-deployment and which must be pushed in production, at-deployment. Solved for this with coffee and configuration testing to confirm.

Again worked with the Development team, this time to define regular expression matching (this was just before AI was being leveraged). Mostly this was fancy 'find and replace'. Thank you, bash. Then, these manipulations were pushed against all build configuration files.

## Insights learned along the way
Each team had a different, specialized skill set. It was fascinating to learn and develop vernacular to meet and elevate each other.

## Learned how to train a group and how to foster a new team mindset
At that point, it was necessary to train the team applying these configurations and getting the boxes out the door. Logistically, this meant that a team of more than a handful needed new documentation and training to scale up the build process by at least 300% - they almost doubled that. Mindset was learned and adopted, and the team got to work. After a few builds, we saw the productivity gains increase rapidly and projections for the deadline were soon well within reach.

## Company culture insights
Since there was so much communication and parallel work tasks to be completed across teams, I learned how to present the needed tasks in a way that was appreciated and valued by management, stakeholders, and teammates. I was honored to see this language used for task delegation pop up across the business.

## Process and configuration validation
Once the build process was churning on its own, I was able to spot-check and QA, identifying any remaining/dynamic items to address. This meant creating a new process and workflow to ensure all boxes moved into production had all remaining QA items addressed to ensure stability and the highest level of Cybersecurity.

# Into production
As these firewalls were being deployed into production, I was grateful that everyone stayed online...and also for such thoughtful and thorough feedback from the team. We used lessons learned to quickly adapt to anything needed and how to dynamically ensure all was in place as needed for this and the next in the fleet.

### Thinking back
It was such a great opportunity to work with the most talented teammates. Even though this project had highest priority for all involved teams, there were limitations on how much time could be used during the technical planning phase. The fleet had since been in full production for over a year, confirming stability and success of the project. Sometimes, we are presented with extraordinary challenges that impact a high volume of people - both coworkers, clients, and their clients; pushing through was rewarding and informed efficiency gains and friendships through the business. It also informed my future projects, taking advantage of these new efficiency gains and high-quality methodology.

Thanks for reading.
