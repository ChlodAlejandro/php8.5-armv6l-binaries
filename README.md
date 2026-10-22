# PHP 8.5.12 for armv6l (Raspberry Pi 1/1B)

These are built PHP 8.5.12 binaries built for a Raspberry Pi 1B.
Sources come from https://packages.sury.org/php/, tweaked to compile
for an armv6l target with a VFPv2 instructions (to suit the RPi's
FPU).

**INSTALLING PACKAGES FROM A RANDOM PERSON IS A BAD IDEA!**

These come at the wake of the recently-released
[critical PHP security update](https://www.php.net/archive/2026.php#2026-10-21-5)
which addressed two CVSS v4.0 9.2 vulnerabilities (CVE-2026-109618 and
CVE-2026-109619). As Raspbian packages are not yet available for 8.5.12
(nor are they available for 8.2.35, as Raspbian appears to track PHP 8.2),
these are freshly compiled from the patched sources on my own computer.

**INSTALLING PACKAGES FROM A RANDOM PERSON IS A BAD IDEA!**

While I'm making them available here, **these are not official packages!**
It's very important that you stick to trusted, official packages from
Raspbian than use some random guy's built `.deb` files. This is only a
stopgap solution for an existing security hole! **These are unsigned
packages and you shouldn't be installing random people's packages on your
computer!**

**INSTALLING PACKAGES FROM A RANDOM PERSON IS A BAD IDEA!**

I don't normally compile PHP or Debian packages in general so this was done
with the assistance of Claude Sonnet 5.5. I've verified each of the commands
I had to run in the terminal for accuracy and safety, because I have eyes
and I think that vibecoding is a plague.

**INSTALLING PACKAGES FROM A RANDOM PERSON IS A BAD IDEA!**

If you want to build your own PHP packages (i.e. ones for PHP versions you
care about), make sure to configure the build to use VPFv2, or else you'll
get SIGILLs trying to run PHP.

# Once official up-to-date PHP packages are available on [Raspbian](https://www.raspbian.org/) via APT, download packages from there.
Follow [this bug](https://bugs.launchpad.net/raspbian/+bug/2171892) on their Launchpad bug tracker for progress.