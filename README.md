Scripts are ran within Power Automate Desktop, process utilizes both Web and Desktop flows <br/>

>The Web flow is started when a MS Form is submitted containing submitted file names<br/>
>>-Submitted files are sent to a Sharepoint folder<br/>
>>-File names contained in JSON, parsed and submitted to PAD*<br/>
>>-Powershell script will convert from Powershell 5 to Powershell 7, create a JSON file with provided variables, and launch Python3<br/>
>>>>-PAD* utilizes Python2 (IronPython 2.7) and Powershell 5, making needed resources unusable<br/>
>>-Python3 will then open the JSON file, parse it, the convert MP3 to WAV and Mono. Then merge the provided audio files into one<br/>
>>-Audio file is then uploaded to 3CX<br/>

PAW = Power Automate Web<br/>
PAD = Power Automate Desktop<br/>
>-Power Automate configuration not available<br/>
<p>Sensative information has been swapped out with *******<br/>
"%variable%" is used as variables that Power Automate feeds into the Powershell script <br/><p/>
