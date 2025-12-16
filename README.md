<img align="right" width="250" height="47" src="../media/Gematik_Logo_Flag.png"/> <br/>


# JMeter

<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
       <ul>
        <li><a href="#release-notes">Release Notes</a></li>
      </ul>
	</li>
    <li>
      <a href="#getting-started">Getting Started</a>
    </li>
    <li>
      <a href="#usage">Usage</a>
    </li>
    <li><a href="#security-policy">Security Policy</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
  </ol>
</details>

## About The Project

This Project should provide a simple means to test the locally running demis kubernetes cluster. 
It is a simple JMeter test script that can be used to test the endpoints of all demis services.
It contains sending pathogen, disease, bedOccupancy and igs fhir Bundles to the demis cluster.
It also allows to retrieve those bundles from the demis cluster.

### Release Notes
See [ReleaseNotes](ReleaseNotes.md) for all information regarding the (newest) releases.

## Getting Started
- Download the latest apache JMeter distribution
- Start the client with a double click on ApacheJMeter.jar or run the jmeter.bat file.
- Load the desired JMX-File(public/demis.jmx).
- Load the _demis.keystore_ into the SSL Manager (Menu/Options/SSL Manager)

For headless testing please consult the official apache JMeter documentation.

## Usage
- You can start the test by clicking on the green play button.
- If JMeter asks you for a password, use "password".
- To show the results click on "_View Results Tree_" or "_Summary Report_".
- To format the result to JSON select the combo box in "_Results Tree". You can find it above the Sample Results entry list.

If your Setup of the [DEMIS-Development-Cluster](https://github.com/gematik/DEMIS-Development-Cluster) was correct you should see that all requests are successful.

Hint: After the the setup script finished it may be possible that you have to wait a few minutes until the demis cluster
is fully up and running due to internal mechanisms not being finisched entirely.

## Security Policy
If you want to see the security policy, please check our [SECURITY.md](.github/SECURITY.md).

## Contributing
If you want to contribute, please check our [CONTRIBUTING.md](.github/CONTRIBUTING.md).

## License

Copyright 2025-2025 gematik GmbH

EUROPEAN UNION PUBLIC LICENCE v. 1.2

EUPL © the European Union 2007, 2016

See the [LICENSE](./LICENSE) for the specific language governing permissions and limitations under the License

## Additional Notes and Disclaimer from gematik GmbH

1. Copyright notice: Each published work result is accompanied by an explicit statement of the license conditions for use. These are regularly typical conditions in connection with open source or free software. Programs described/provided/linked here are free software, unless otherwise stated.
2. Permission notice: Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
   1. The copyright notice (Item 1) and the permission notice (Item 2) shall be included in all copies or substantial portions of the Software.
   2. The software is provided "as is" without warranty of any kind, either express or implied, including, but not limited to, the warranties of fitness for a particular purpose, merchantability, and/or non-infringement. The authors or copyright holders shall not be liable in any manner whatsoever for any damages or other claims arising from, out of or in connection with the software or the use or other dealings with the software, whether in an action of contract, tort, or otherwise.
   3. We take open source license compliance very seriously. We are always striving to achieve compliance at all times and to improve our processes. If you find any issues or have any suggestions or comments, or if you see any other ways in which we can improve, please reach out to: ospo@gematik.de
3. Please note: Parts of this code may have been generated using AI-supported technology. Please take this into account, especially when troubleshooting, for security analyses and possible adjustments.

## Contact
E-Mail to [DEMIS Entwicklung](mailto:demis-entwicklung@gematik.de?subject=[GitHub]%20JMeter)
