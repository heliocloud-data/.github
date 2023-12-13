## Greetings 👋

Welcome to the HelioCloud:  An open-source, cloud-base analytics and data platform for empowering heliophysics research. You probably came here by way of our public site https://heliocloud.org,  but if not we suggest you stop there first and take a look around.  We also use [heliocloud@groups.io](https://groups.io/g/heliocloud) for assisting in HelioCloud installation.

Like other great open-souce projects, we've chosen to host the HelioCloud codebase on GitHub to maximize accesibility for the HelioPhysics community, encouraging dialogue, participation and community code contributions.  Please dive in and tell us what you think!

To access the publicly-available terabytes of AWS-stored heliophysics datasets, run 'pip install cloudcatalog' and follow our examples in the 'Tutorials' repo.

To build a HelioCloud, the basic steps are: on/after Dec 11th, download the platform from our public GitHub.  Run the supplied cdk scripts to install the daskhub environment/jupyter setup/PyHC-based containers.  You are then the admin and can add users, who will have both a private disk area and a disk area shared by all users on your instance.

Below is a breakdown of the core installation steps as an overview.  If there are steps you need help with (for example, on my first install I needed help installing CDK), we have additional documentation and we’re happy to work with you.  This summary list is just to lay out the pieces so we’re starting at the same place.  

1. Pre-configuration steps:
   * Get an AWS account from AWS and save your AWS credentials for the install.
   * Install Python 3.9 or later, Docker, the AWS Command Line Interface (CLI), and AWS CDK (requires npm and Node.js)
2. Do a 'git clone' of the 'platform' repository.
3. 'cd' into the repo and run the supplied CDK scripts to install the daskhub environment/jupyter setup/PyHC-based containers.
4. As admin, set up user accounts for researchers who will be working on your HelioCloud instance.

A single HelioCloud deployment into an AWS account is referred to as a HelioCloud instance, in keeping with the idea that you are instantiating a HelioCloud using a certain set of parameters as provided by your instance's configuration file. Only one person is needed for the 'admin' role that requires a billable AWS account.  (You then create a Cognito pool for your researchers/students and send out invitations for them to join.  Individual users therefore do not need an AWS account.)

## TODO:  Sections we will be adding
🌈 Contribution guidelines - how can the community get involved?
👩‍💻 Useful resources - where can the community find your docs? Is there anything else the community should know?
