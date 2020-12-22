
This is an adapted version of drmon written by aedan. It has been modified to use the algoritm and positions from OmegaPhi115.
![](examples/2.jpg)
> *status*: currently in development


# drmon
Monitor and failsafe automation for your draconic reactor.

# Bat
Monitor for Draconic Storage.

# Pocket
Remote access to reactor controls and monitoring.

### What is this
This is a set of computercraft LUA scripts that monitors everything about a draconic reactors and storage, with a couple features to help keep it from exploding
NB: This is for Minecraft 1.12.2. You will need to answer some questions on console during install.


### Tutorial
1.7.10: You can find a very well made youtube tutorial on how to set this up [here](https://www.youtube.com/watch?v=8rBhQP1xqEU), thank you [The MindCrafters](https://www.youtube.com/channel/UCf2wEy4_BbYpAQcgvN26OaQ).

I have not created a tutorial for 1.12.2 yet.

### Features
* Uses a 3x3 advanced computer touchscreen monitor to interact with your reactor
* Automated regulation of the input gate for the targeted field strength of 50%
* Immediate shutdown and charge upon your field strength going below 25%
  * Reactor will activate upon a successful charge
* Immediate shutdown when your temperature goes above 8000C
  * Reactor will activate upon temperature cooling down to 7000C
* Easily tweak your output flux gate via touchscreen buttons
  * +/-100k, 10k, and 1k increments
* Monitor storage cell capacity on 3x3 screen connected the same way as reactor monitoring
* Remote monitoring is available via ender modems(optional)
  * Remote monitoring can monitor multiple reactors at once.
  * Allows for remote status, shutdown, startup of reactors and patching

### Requirements:
* One fully setup draconic reactor (and fuel, obviously);
* 1 advanced computer;
* 9 advanced monitors;
* 3 wired modems, wireless will not work;
* A bunch of network cables;
* 1 ender modem (Optional);

### Installation:
* Your reactor output flux gate must be setup so that one side of it and one of your stabilizers touches a side of the advanced computer;
* By default, flux gate should touch the top side, stabilizer on the left of the computer;
  * If you want to use different sides you need to modify `startup` after you have installed this and specify the sides;
* Connect a modem to your input flux gate (the one connected to your reactor energy injector);
* Connect a modem to your advanced computer (at the botom side);
* Setup your monitors to be a 3x3 and connect a modem to anywhere but the front;
* Run network cable to all 3 modems;
* Install this code via running the install script using these commands:

```
> pastebin get mgF6RZFQ startup
> startup

> On Advanced ender pocket computer (Optional)
> pastebin get PUWxdYWY startup
> startup
```

* You should see stats in your term, and on your monitor

### Upgrading to the latest version
* Right click your computer;
* Hold ctrl+t until you get a `>`;

```
> reboot
```

### Known issues
* There is a problem with **skyfactory 2.5** and **pastebin**, see workarounds [here](https://github.com/acidjazz/drmon/issues/9#issuecomment-277910288).
