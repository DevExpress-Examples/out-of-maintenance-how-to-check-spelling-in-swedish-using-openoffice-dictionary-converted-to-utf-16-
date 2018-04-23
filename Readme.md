# How to check spelling in Swedish using OpenOffice dictionary converted to UTF-16


<p>This example demonstrates how to check Swedish spelling in Silverlight application using currently available OpenOffice dictionary.<br />
Since <strong>Silverlight</strong> platform currently supports only <strong>utf-8</strong> and <strong>utf-16</strong> encodings, you cannot use OpenOffice dictionary as-is. It should be converted first to an encoding recognizable by Silverlight application. This example utilizes dictionary in UTF-16 (Unicode) encoding.</p><p>To get OpenOffice Swedish dictionary ready for use with Silverlight, perform the following steps: </p><p>Download OpenOffice dictionary at <u><a href="http://extensions.services.openoffice.org/project/dict-sv">http://extensions.services.openoffice.org/project/dict-sv</a></u> page.<br />
Change its extension to .zip.<br />
Extract all files. <br />
Find sv_SE.aff and sv_SE.dic in the <strong>dictionaries </strong>folder.<br />
Get the <strong>CodePageConverter_UTF16</strong> utulity. You can find it in the <a href="https://www.devexpress.com/Support/Center/p/K18404">K18404: How to use Open Office dictionaries to check spelling in different languages</a> KnowledgeBase article.<br />
Run it in a folder that contains .dic and .aff files.<br />
Use resulting sv_SE_utf16.dic and sv_SE_utf16.aff files in your project.</p><p>Note that the <strong>Encoding</strong> property of the dictionary should be set to <strong>Encoding.Unicode</strong> before a dictionary is loaded.</p>

<br/>


