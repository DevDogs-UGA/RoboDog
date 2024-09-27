# What is RoboDog?
RoboDog is a Discord bot providing an additional interface for the internal [DevDogs Platform](https://github.com/DevDogs-UGA/DevDogs-Platform), 
which powers RoboDog and the [DevDogs Website](https://github.com/DevDogs-UGA/DevDogs-Website), and automation of common administrative actions.

## Goals
RoboDog is in *very* early stages of development, so below are some goals to achieve with this project before they manifest as GitHub Issues:

- Enforce server nickname conventions using existing member profile data
  - Recognize existing members on join, adjusting database records accordingly
- Provide a command to link users' many accounts internally
  - Request linking (and verify) through DMs on server join
- Automate frequent tasks like event/meeting setup
  - Auto-start stage channel, stage thread, and post of audience instructions
- Anonymous enforcement of server and club rules (warnings and other moderation features)
- Provide a command to request repo access, with respect to a member's focus group designation, year, and server roles
- Provide commands for superiors to retrieve member statistics
- Provide commands to force-add points and amend non-code or other untracked contributions
- Automate transition-of-power, onboarding, and termination of "employment" tasks

## How It'll Work
### (A Very Brief Look At) Architecture
This repository strictly hosts the code powering the Discord *interface* and any Discord-only functionalities. Member data, contribution processing, and
other critical processes are managed by the [DevDogs Platform](https://github.com/DevDogs-UGA/DevDogs-Platform), which powers our website too. Users
will interact with this program, which receives, interprets, then acts upon commands. RoboDog-provided functionalities such as nickname enforcement
are handled by this program, with other, DevDogs-critical functionalities like contribution management relegated to the DevDogs Platform program so
changes are reflected across both end-user interfaces (the website and Discord).

### Contributing
This repository, in the future, will be managed by a titled Discord developer unless the role is integrated with the Lead Web Developer under a title change 
(Lead Web Developer -> DevDogs Platform Developer). This repository, after setup, can be contributed to by general body members of DevDogs as another 
valid, points-rewarding "Side Quest."
