.. RedVox Website Examples documentation master file, created by
   sphinx-quickstart on 2022 Jun 7.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.


Redvox Website Examples
================================

Welcome to Redvox Website Examples!

This is a space for examples and tutorials of the RedVox website at `redvox.io <https://redvox.io/#/home>`_.

The RedVox website is the portal to RedVox data and aggregated reports.  Reports are precompiled sets of RedVox data
that detail an event of interest.  These examples will walk you through the process of navigating the website and
downloading data to work with.

Contents
----------

**Setup**

- :doc:`prereqs`

**redvox.io**

- :doc:`00_redvox_website`
- :doc:`01_account`
- :doc:`02_dashboard`
- :doc:`03_report`

Basic definitions
------------------

The following terms are common terminology used throughout this documentation.

- **RedVox**: Not the NYC based rock band. RedVox refers to products developed by `RedVox, Inc. <http://nelha.hawaii.gov/our-clients/redvox/>`_.

- **redvox.io**: the RedVox webpage where RedVox reports are done. Visit `redvox.io <https://redvox.io/#/home>`_.

- **RedVox Report**: `redvox.io <https://redvox.io/#/home>`_ can perform the sensor analysis
  (plot audio waveforms, spectrograms, state of health data) for you and provide a summary - a report.

- **RedVox Infrasound Recorder**: A smartphone app that can record audio and other stimuli such as pressure.
  Visit `RedVox Sound <https://www.redvoxsound.com>`_ to learn more about the app.

- **RedVox Python SDK**: A Software Development Kit (SDK) developed to read, create, edit, and write RedVox files
  (files ending in `.rdvxz` for `RedVox API 900 <https://bitbucket.org/redvoxhi/redvox-protobuf-api/src/master/>`_
  files and `.rdvxm` for `RedVox API 1000 <https://github.com/RedVoxInc/redvox-api-1000>`_ files). Visit
  `GitHub RedVox Python SDK <https://github.com/RedVoxInc/redvox-python-sdk>`_ to learn more about the SDK.

- **Station**: a device used to record data, e.g., a smartphone recording infrasound waves using the
  `RedVox Infrasound Recorder <https://www.redvoxsound.com/>`_ app. Also a Python class designed in the RedVox Python SDK to
  store station and sensor data. Visit
  `Station Documentation <https://github.com/RedVoxInc/redvox-python-sdk/tree/master/docs/python_sdk/data_window/station>`_
  for more information on the Station Python class. A station has sensors (see below).

- **Sensor**: a device that responds to a physical stimulus, e.g., barometer, accelerometer. The units for each available sensor can
  be found in `RedVox SDK Sensor Documentation <https://github.com/RedVoxInc/redvox-python-sdk/tree/master/docs/python_sdk/data_window/station#sensor-data-dataframe-access>`_.
  A station should always have audio sensor (and hence audio data).

- **Epoch** or **epoch time**: unix time (also referred to as the epoch time), the number of seconds since 1 January 1970.
  For example the epoch time for Thursday, July 1, 2021 at 9:00:00 am UTC would be 1625130000.

.. toctree::
   :maxdepth: 2
   :caption: Before Starting...
   :hidden:

   prereqs

.. toctree::
   :maxdepth: 2
   :hidden:
   :caption: redvox.io...

   00_redvox_website
   01_account
   02_dashboard
   03_report

.. toctree::
   :maxdepth: 2
   :hidden:
   :caption: For more information:

   what_to_do_next
   troubleshooting
