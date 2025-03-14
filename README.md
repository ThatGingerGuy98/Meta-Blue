# Meta-Blue
An open source hunt framework for Microsoft Windows networks. Find out your network's host configuration baseline and what lies outside of it on the fly. 

Currently collects 76 forensically relevant data points.

# Command Line arguments
Meta-Blue supports some basic command line arguments that allow the script to run without user interaction.  You can use `-help` in the command line to see this message.
    `Meta-Blue (no args): Launches Meta-Blue in interactive mode.`
    
    `Meta-Blue -enum    : Launches in enumeration.`
    
    `Meta-Blue -coll    : Launches in collection.`
    
    `Meta-Blue -local   : Runs Meta-Blue against the local box.`
    
    `Meta-Blue -help    : Shows this help message.`
    
    `-help can be used after the first argument to show help for that argument.`
    
    `Add "-json" anywhere within the arguments to output the results in JSON format.`

# In Progress:

## Collection
 - A few of the datapoints being collected are either irrelevant or do not return something of implict value.
 - Reworking services to scrape registry instead of get-services/gwmi win32_service/etc.
 - Incorporating checks from tools like [WinPwn](https://github.com/S3cur3Th1sSh1t/WinPwn) and [WinPEAS](https://github.com/peass-ng/PEASS-ng/tree/master/winPEAS). (if attackers know where they can privesc, shouldn't you?)

## UI/UX
 - Finally working on getting rid of the menu.
 - Using cmdletbinding in next version
