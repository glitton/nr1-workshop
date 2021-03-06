# workshop/lab9

This repo has been spun up locally only.

## Getting started

1. Open a Terminal window.
2. Type the following to confirm that you can run the NR1 CLI `nr1 --version`
3. If you can't run that command, go to the **Build your own application** launcher in New Relic One, register for a developer API key and download the NR1 CLI. See the complete [Setup instructions](../SETUP.md) for more details
4. Open a Terminal window. From the command line you should the following:

```bash
# To verify that you've unzipped the NR1 CLI, run this command and see similar output
ls ~/nr1
README.md node_modules package-lock.json bin oclif.manifest.json package.json
```

5. From the command line, run the following:

```bash
#Create an alias to the cli
ln -s ~/nr1/bin/nr1 /usr/local/bin/nr1

#Verify that you can execute nr1
nr1 --version

#You should see output to the terminal window
```

6. And if you haven't already cloned the workshop repo, do that now.

```bash
# if you haven't cloned the workshop repo already
git clone git@github.com:newrelic/nr1-workshop.git

# then change directory into lab9
cd workshop/lab9

nr1 nerdpack:uuid -gf
npm install
npm start
```

8. In Google Chrome, navigate to the following URL `https://one.newrelic.com?nerdpacks=local`

1. In Google Chrome, navigate to `https://github.com/newrelic/eap-cli/tree/master/dist`, and click on the latest release of the NR1 CLI. (ex. `nr1-v0.3.0-alpha.11`)
2. Download the apppropriate zipped bundle of the NR1 CLI and **unzip it to your home folder** (ex. for Mac it would be `nr1-v0.3.0-alpha.11-darwin-x64.tar.gz`).
3. Open a Terminal window. From the command line you should the following:

```bash
# To verify that you've unzipped the NR1 CLI, run this command and see similar output
ls ~/nr1
README.md node_modules package-lock.json bin oclif.manifest.json package.json
```

4. From the command line, run the following:

```bash
#Create an alias to the cli
ln -s ~/nr1/bin/nr1 /usr/local/bin/nr1

#Verify that you can execute nr1
nr1 --version

#You should see output to the terminal window
```

5. If you haven't done so yet, generate your personal SSL cert for your development environment.

```bash
cd ~
sudo ./nr1/bin/nr1 certs:generate
#The cert will be saved to a hidden folder
```

6. And if you haven't already cloned the workshop repo, do that now.

```bash
# if you haven't cloned the workshop repo already
git clone git@github.com:newrelic/nr1-workshop.git

# then change directory into lab9
cd workshop/lab9
nr1 nerdpack:uuid -gf
npm install
npm start
```

7. In Google Chrome, navigate to the following URL `https://one.newrelic.com?nerdpacks=local`

## Lab Instructions

[Everything you wanted to know about NerdStorage _but were afraid to ask_](INSTRUCTIONS.md).