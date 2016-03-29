<snippet>
  <content>
#PersonalPool
PersonalPool is a fork of Vanitygen, a command line tool for creating vanity bitcoin addresses, now available to deploy on multiple computers for a 'personal pool.'

The adaptation is currently in progress, this repo is not useful yet!

Heavily adapted by me to run on friends' computers with their explicit consent to reduce the time it takes me to find bitcoin vanity addresses.  The Vanitygen software uses the host computer's GPU to make millions of random bitcoin addresses, discarding the vast majority until ones with a predetermined pattern are found. Running the script begins a process on as many threads as there are on the CPU (this can be lowered to 1 thread). Eventually, you'll stumble upon an address that has a pattern to it, like ILOVEYOU or other seemingly non-random but are actually valid 'random' strings of text.

Finding and address with a "1" in it is easy. Finding "1A" is also simple, you might get a pattern with that in just a few hundred generations of bitcoin addresses, at which point you could stop. Due to math, the computational power required to find an address more than 8 or 9 characters long becomes unbearable.

Use the tools in this repo to make a cloud/pool of computers, stopping only when one computer finds the desired vanity address. A flask server is run on the administrators computer, listening on a REST API for reports from any currently running the Vanitygen client.

## Usage
Step 1: As the admin/host computer you'll need to make sure the Flask server is running so you're listening for the reports from the clients. I had to setup port forwarding on my router, and I use the dynamic dns updating feature to make sure my domain will always reach my server. Find Flask tutorials, it's very simple.

Step 2: Setup your client config, choose your vanity address in the TODO: add dedicated config file. Remember addresses must start with 1, and it doesn't make sense to try making a vanity address with too many characters. Don't be rude and make a bunch of friends and family search day and night for an address that can't be found for hundreds of years, so go figure out vanitygen
I use 64bit because it's quite a bit faster. Change this according to the rate of your client's CPU.
TODO: Add a dedicated config file

Step 3: TODO

##FAQs
Why does the .

</content>
</snippet>