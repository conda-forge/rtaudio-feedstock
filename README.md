About rtaudio
=============

Home: https://www.music.mcgill.ca/~gary/rtaudio/

Package license: MIT

Feedstock license: [BSD-3-Clause](https://github.com/conda-forge/rtaudio-feedstock/blob/main/LICENSE.txt)

Summary: Cross-platform C++ API for realtime audio input/output

Development: https://github.com/thestk/rtaudio

Documentation: https://www.music.mcgill.ca/~gary/rtaudio/index.html

RtAudio is a set of C++ classes that provides a common API (Application Programming Interface) for realtime audio input/output across Linux (native ALSA, JACK, PulseAudio and OSS), Macintosh OS X and Windows (DirectSound, ASIO and WASAPI) operating systems. RtAudio significantly simplifies the process of interacting with computer audio hardware. It was designed with the following objectives:

    - object-oriented C++ design
    - simple, common API across all supported platforms
    - only one source and one header file for easy inclusion in programming
        projects
    - allow simultaneous multi-api support
    - support dynamic connection of devices
    - provide extensive audio device parameter control
    - allow audio device capability probing
    - automatic internal conversion for data format, channel number
        compensation, (de)interleaving, and byte-swapping

RtAudio incorporates the concept of audio streams, which represent audio output (playback) and/or input (recording). Available audio devices and their capabilities can be enumerated and then specified when opening a stream. Where applicable, multiple API support can be compiled and a particular API specified when creating an RtAudio instance.


Current build status
====================


<table>
    
  <tr>
    <td>Azure</td>
    <td>
      <details>
        <summary>
          <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=18395&branchName=main">
            <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/rtaudio-feedstock?branchName=main">
          </a>
        </summary>
        <table>
          <thead><tr><th>Variant</th><th>Status</th></tr></thead>
          <tbody><tr>
              <td>linux_64</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=18395&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/rtaudio-feedstock?branchName=main&jobName=linux&configuration=linux%20linux_64_" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>linux_aarch64</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=18395&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/rtaudio-feedstock?branchName=main&jobName=linux&configuration=linux%20linux_aarch64_" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>linux_ppc64le</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=18395&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/rtaudio-feedstock?branchName=main&jobName=linux&configuration=linux%20linux_ppc64le_" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>osx_64</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=18395&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/rtaudio-feedstock?branchName=main&jobName=osx&configuration=osx%20osx_64_" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>osx_arm64</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=18395&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/rtaudio-feedstock?branchName=main&jobName=osx&configuration=osx%20osx_arm64_" alt="variant">
                </a>
              </td>
            </tr><tr>
              <td>win_64</td>
              <td>
                <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=18395&branchName=main">
                  <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/rtaudio-feedstock?branchName=main&jobName=win&configuration=win%20win_64_" alt="variant">
                </a>
              </td>
            </tr>
          </tbody>
        </table>
      </details>
    </td>
  </tr>
</table>

Current release info
====================

| Name | Downloads | Version | Platforms |
| --- | --- | --- | --- |
| [![Conda Recipe](https://img.shields.io/badge/recipe-librtaudio6-green.svg)](https://anaconda.org/conda-forge/librtaudio6) | [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/librtaudio6.svg)](https://anaconda.org/conda-forge/librtaudio6) | [![Conda Version](https://img.shields.io/conda/vn/conda-forge/librtaudio6.svg)](https://anaconda.org/conda-forge/librtaudio6) | [![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/librtaudio6.svg)](https://anaconda.org/conda-forge/librtaudio6) |
| [![Conda Recipe](https://img.shields.io/badge/recipe-rtaudio-green.svg)](https://anaconda.org/conda-forge/rtaudio) | [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/rtaudio.svg)](https://anaconda.org/conda-forge/rtaudio) | [![Conda Version](https://img.shields.io/conda/vn/conda-forge/rtaudio.svg)](https://anaconda.org/conda-forge/rtaudio) | [![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/rtaudio.svg)](https://anaconda.org/conda-forge/rtaudio) |

Installing rtaudio
==================

Installing `rtaudio` from the `conda-forge` channel can be achieved by adding `conda-forge` to your channels with:

```
conda config --add channels conda-forge
conda config --set channel_priority strict
```

Once the `conda-forge` channel has been enabled, `librtaudio6, rtaudio` can be installed with `conda`:

```
conda install librtaudio6 rtaudio
```

or with `mamba`:

```
mamba install librtaudio6 rtaudio
```

It is possible to list all of the versions of `librtaudio6` available on your platform with `conda`:

```
conda search librtaudio6 --channel conda-forge
```

or with `mamba`:

```
mamba search librtaudio6 --channel conda-forge
```

Alternatively, `mamba repoquery` may provide more information:

```
# Search all versions available on your platform:
mamba repoquery search librtaudio6 --channel conda-forge

# List packages depending on `librtaudio6`:
mamba repoquery whoneeds librtaudio6 --channel conda-forge

# List dependencies of `librtaudio6`:
mamba repoquery depends librtaudio6 --channel conda-forge
```


About conda-forge
=================

[![Powered by
NumFOCUS](https://img.shields.io/badge/powered%20by-NumFOCUS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A)](https://numfocus.org)

conda-forge is a community-led conda channel of installable packages.
In order to provide high-quality builds, the process has been automated into the
conda-forge GitHub organization. The conda-forge organization contains one repository
for each of the installable packages. Such a repository is known as a *feedstock*.

A feedstock is made up of a conda recipe (the instructions on what and how to build
the package) and the necessary configurations for automatic building using freely
available continuous integration services. Thanks to the awesome service provided by
[Azure](https://azure.microsoft.com/en-us/services/devops/), [GitHub](https://github.com/),
[CircleCI](https://circleci.com/), [AppVeyor](https://www.appveyor.com/),
[Drone](https://cloud.drone.io/welcome), and [TravisCI](https://travis-ci.com/)
it is possible to build and upload installable packages to the
[conda-forge](https://anaconda.org/conda-forge) [Anaconda-Cloud](https://anaconda.org/)
channel for Linux, Windows and OSX respectively.

To manage the continuous integration and simplify feedstock maintenance
[conda-smithy](https://github.com/conda-forge/conda-smithy) has been developed.
Using the ``conda-forge.yml`` within this repository, it is possible to re-render all of
this feedstock's supporting files (e.g. the CI configuration files) with ``conda smithy rerender``.

For more information please check the [conda-forge documentation](https://conda-forge.org/docs/).

Terminology
===========

**feedstock** - the conda recipe (raw material), supporting scripts and CI configuration.

**conda-smithy** - the tool which helps orchestrate the feedstock.
                   Its primary use is in the construction of the CI ``.yml`` files
                   and simplify the management of *many* feedstocks.

**conda-forge** - the place where the feedstock and smithy live and work to
                  produce the finished article (built conda distributions)


Updating rtaudio-feedstock
==========================

If you would like to improve the rtaudio recipe or build a new
package version, please fork this repository and submit a PR. Upon submission,
your changes will be run on the appropriate platforms to give the reviewer an
opportunity to confirm that the changes result in a successful build. Once
merged, the recipe will be re-built and uploaded automatically to the
`conda-forge` channel, whereupon the built conda packages will be available for
everybody to install and use from the `conda-forge` channel.
Note that all branches in the conda-forge/rtaudio-feedstock are
immediately built and any created packages are uploaded, so PRs should be based
on branches in forks and branches in the main repository should only be used to
build distinct package versions.

In order to produce a uniquely identifiable distribution:
 * If the version of a package **is not** being increased, please add or increase
   the [``build/number``](https://docs.conda.io/projects/conda-build/en/latest/resources/define-metadata.html#build-number-and-string).
 * If the version of a package **is** being increased, please remember to return
   the [``build/number``](https://docs.conda.io/projects/conda-build/en/latest/resources/define-metadata.html#build-number-and-string)
   back to 0.

Feedstock Maintainers
=====================

* [@ryanvolz](https://github.com/ryanvolz/)

