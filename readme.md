<body>
    <table class="TOC">
        <tr>
            <th>
                <strong>Table of Contents</strong>
            </th>
        </tr>
        <tr>
            <td>
                <a href="#Welcome">Welcome</a>
            </td>
        </tr>
        <tr>
            <td>
                <a href="#Package">Package Contents</a>
            </td>
        </tr>
        <tr>
            <td>
                <a href="#Syntax">Syntax</a>
            </td>
        </tr>
        <tr>
            <td>
                <a href="#ErrorLevel">Return Codes</a> (ERRORLEVEL)
            </td>
        </tr>
        <tr>
            <td>
                <a href="#HowTo">How To...</a>
            </td>
        </tr>
    </table>
    <p>
        &nbsp;
    </p>
    <hr />
    <a id="Welcome" />
    <h2>Welcome</h2>
    <div class="h2content">
        <p>
            <strong>Display is a small command-linetool that allows you to either change display orientation or to change the brightness or the contrast of a specified display device (if supported by the display driver and the system) or to turn the monitors or the screen saver on and off to save power.
        </p>
        <p><strong>Notes:</strong></p>
        <ul>
            <li>
                Both the <em>display32.exe</em> and <em>display64.exe</em> executable files don't have any runtime dependencies so they can be easily copied to a USB stick if needed to be used on other systems.
            </li>
        </ul>
    </div>
    <hr />
    <a id="Package" />
    <h2>Package Contents</h2>
    <div class="h2content">
        <p>
            The package is provided as a compressed (zip) archive that holds a few files. The
            included files are described in the table below.
        </p>
        <table class="description">
            <tr>
                <th>File</th>
                <th>Description</th>
            </tr>
            <tr>
                <td style="text-align: center">display32.exe</td>
                <td>The Display program (32-bit version)</td>
            </tr>
            <tr>
                <td style="text-align: center">display64.exe</td>
                <td>The Display program (64-bit version)</td>
            </tr>
            <tr>
                <td style="text-align: center">readme.htm</td>
                <td>This file.</td>
            </tr>
        </table>
    </div>
    <hr />
    <a id="Syntax" />
    <h2>Syntax</h2>
    <div class="h2content">
        <p>
            Display features many parameters, for a whole list of the supported parameters and
            a description, type the following command in a <em>Command</em> window:
        </p>
        <pre>display32 /?</pre>
        <p>
            <strong>Examples:</strong>
        </p>
        <ul>
            <li>
                <p>
                    To turn all the monitors off, use:
                </p>
                <pre>display32 /power off</pre>
            </li>
            <li>
                <p>
                    To rotate the display orientation of monitor #2 by 90° counter-clockwise, use:
                </p>
                <pre>display32 /device 2 /rotate 90</pre>
            </li>
        </ul>
    </div>
    <hr />
    <a id="ErrorLevel" />
    <h2>Return Codes (ERRORLEVEL)</h2>
    <div class="h2content">
        <p>
            When Display is used in a batch file, you can use <em>ERRORLEVEL</em> to check the
            completion code returned by the program. The possible return codes are listed in
            the table below.
        </p>
        <table class="description" style="width: 70%">
            <tr>
                <th style="width: 20%">
                    Code
                </th>
                <th>
                    Description
                </th>
            </tr>
            <tr>
                <td style="text-align: center">
                    0
                </td>
                <td>
                    Success.
                </td>
            </tr>
            <tr>
                <td style="text-align: center">
                    1
                </td>
                <td>Syntax error or help/registration information displayed.</td>
            </tr>
            <tr>
                <td style="text-align: center">
                    2
                </td>
                <td>
                    General failure.
                </td>
            </tr>
            <tr>
                <td style="text-align: center">
                    3
                </td>
                <td>
                    Unable to adjust brightness.
                </td>
            </tr>
            <tr>
                <td style="text-align: center">
                    4
                </td>
                <td>
                    Unable to adjust contrast.
                </td>
            </tr>
            <tr>
                <td style="text-align: center">
                    5
                </td>
                <td>
                    Unable to set display orientation or position.
                </td>
            </tr>
        </table>
    </div>
    <hr />
    <a id="HowTo" />
    <h2>How To Create a Shortcut To Toggle Display Orientation?</h2>
    <div class="h2content">
        <ul>
            <li>right-click the Desktop</li>
            <li>click <strong>New</strong> &gt; <strong>Shortcut</strong></li>
            <li>click <strong>Browse</strong></li>
            <li>select <strong>display32.exe</strong></li>
            <li>click <strong>OK</strong></li>
            <li>put a blank after the path and append the two parameters: <strong>/rotate 90 /toggle</strong><br />
                <p>e.g. <strong>"C:\MyTools\display32.exe" /rotate 90 /toggle</strong></p>
                <p>Note: quotes are required if the path contains blanks.</p>
            </li>
            <li>click <strong>Next</strong></li>
            <li>give the shortcut a name e.g. <strong>Toggle Display Orientation</strong></li>
            <li>click <strong>Finish</strong></li>
            <li>Pin the new shortcut to the taskbar</li>
        </ul>
    </div>
    <hr />
</body>
</html>
