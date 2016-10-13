ManyWho Box Service Examples
============================

These flows are examples of how to use Box with ManyWho.

## Usage

**Upload a file Example**

Import the flow (example-upload-file.json) into your ManyWho account, you will need an account into box.
Run the flow and upload a file, you will be able to see the properties of the file, and also check that the file will be upload in you root folder in box.

**Example: Listener**

Import the flow (example-listener.json) and run the flow, you will need to Grant access to Box.
You will be asked to "Insert File ID From Box" get the *id of one of your files from box, and paste it at the input field in your flow.
Click in `Go`, you will see the loading symbol (with message `Waiting for step: Load File: with listener`). When you download that file the flow will continue and will show `The File have been downloaded !!!`

**Example: Launch Flow From Box**

For this example is needed an Enterprise Account in Box.
Import the flow (example-launch-flow-from-box.json), Update the value `Enterprise Id` with your own Enterprise Id. And after update the service.
You should authorize manywho_server-to-server and install https://app.box.com/services/manywho (follow instructions in the wiki)
Click in run flow and get the url it should look like this: https://flow.manywho.com/f06c20ee-3702-466c-8437-9b399673f773/play/default?flow-id=yyyy&flow-version-id=xxx
From you box account, click in the `...` symbol, `More Actions` and `Launch Flow ManyWho (directly)` in the ManyWho Flow paste the url copied in the step before, and in Event Trigger type `FILE.DOWNLOADED`.
Click in `CONFIRM FLOW ASSIGNATION` you will see  `Your Flow have been assigned! Please close this tab.`
Download the file that you have select, and refresh the page. The file should have two new task. One with name webhook-target-id and the other with the webhook-target-type.

**Example: Create Task and Assignment **
Import the flow (example-create-task-and-assignment.json), Run the flow.
You will need to type the *id of a file from box, and the email of someone of your box organization.

*How to get the **id of a file from Box**: 

Click in one of your box files the url should look like https://app.box.com/files/0/f/0/1/f_97231111234, you should copy the number after the f_ (in this example is `97231111234`)

### More info

You can have more information of how to configure this service follow the instructions in https://github.com/manywho/service-box/wiki
If you need to deploy the service in your oun environment you can find the code in https://github.com/manywho/service-box

## Contributing

Contribution are welcome to the project - whether they are feature requests, improvements or bug fixes! Refer to 
[CONTRIBUTING.md](CONTRIBUTING.md) for our contribution requirements.

## License

This service is released under the [MIT License](http://opensource.org/licenses/mit-license.php).
