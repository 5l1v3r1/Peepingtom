This project is no longer supported. I have decided to discontinue development due to the success of [EyeWitness](https://github.com/ChrisTruncer/EyeWitness). I figure if I'm abandoning my own tool to use something else, I should probably recommend others do it as well. Enjoy! Thank you.

---

### Usage

1. Install the pre-requisites.

    - cURL
    - PhantomJS:
        - Download or compile PhantomJS v2.X and place the binary in the same directory as the PeepingTom source files.
        - Make sure the binary is named "phantomjs".

2. Run the script.

    - `python ./peepingtom.py -h`

### Notes

- Input is limited only to what PhantomJS allows. PhantomJS will take any string as input for the location of a resource. If a protocol is not given, PhantomJS assumes the string is a file path on the local operating system. Ports apply as normal.

### Changelog

01.07.16

- discontinued development and dropped support for the project.

02.19.15

- migrated capture.js to phantomjs v2.0.
- optimized capture.js to account for several phantomjs error conditions.
- added some code for debugging capture.js in standalone conditions.

05.22.14

- added the ability to specify an output folder.

01.03.14

- migrated from optparse to argparse.

12.13.13

- fixed the indefinite timeout bug in the cURL command.

11.07.13

- added the ability to store and view the source code of each target.
- changed the cURL command to avoid using HEAD requests.

08.09.13

- added the ability to import Nmap files.
- changed the "-n" argument to "-x" for XML input mode.

07.03.13

- removed PyQt4 support.
- completely reorganized and optimized the codebase.
- passed input requirements to PhantomJS. Input is now limited only to what PhantomJS allows (see Notes).
- added the ability to import Nessus files.
- added the ability to screenshot local files.
- added full header infromation for all redirects and the final destination.
- added clickable images for full size viewing.
- added dynamic resizing of the html report.
- added an option for setting the socket timeout.
- modified reporting to group and sort results based on hash values of screenshot images.

11.26.12

- cleaned up the code for release.

07.15.12

- no longer freezes on redirects to 401 authentication.
- stores each run in a unique directory.
- shows headers for final destination rather than redirect.
- denotes redirect next to the status header.