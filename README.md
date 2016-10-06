ManyWho Box Service Examples
============================

These flows are examples of how to use Box with ManyWho.

## Usage

**Upload a file Example.json**

Import the flow into your ManyWho account, you will need an account into box.

**Listener Example Flow**

Import the flow into your ManyWho account, you will need an account into box.
When you run the flow you will be asked to introduce the file id, to get the file id you just need to go to your box account and click in one of your files (or upload a new file), the url of your browser will look like this:
https://app.box.com/files/0/f/0/1/f_97231111234 copy the number after the f_, in this example is `97231111234` and paste it at the input field in your flow.
Click in `LOAD FILE`, you will see the loading symbol (with message `Waiting for step: Load File With Listener`). When you download that file the flow will contine and will show `The File have been downloaded !!!`

**Launch a ManyWho Flow from Box Example**

Import the flow into your ManyWho account, you will need an enterprise account into box. Update the value `Enterprise Id` with your own Enterprise Id. And after update the service.
You should authorize manywho_server-to-server and install https://app.box.com/services/manywho (follow instructions in the wiki)
Click in run flow and get the url it should look like this: https://flow.manywho.com/f06c20ee-3702-466c-8437-9b399673f773/play/default?flow-id=yyyy&flow-version-id=xxx
From you box account, click in the `...` symbol, `More Actions` and `Launch Flow ManyWho (directly)` in the ManyWho Flow paste the url copied in the step before, and in Event Trigger type `FILE.DOWNLOADED`.
Click in `CONFIRM FLOW ASSIGNATION` you will see  `Your Flow have been assigned! Please close this tab.`
Download the file that you have select, and refresh the page. The file should have two new task. One with name webhook-target-id and the other with the webhook-target-type.


### More info

You can have more information of how to configure this service follow the instructions in https://github.com/manywho/service-box/wiki
If you need to deploy the service in your oun environment you can find the code in https://github.com/manywho/service-box

## Contributing

Contribution are welcome to the project - whether they are feature requests, improvements or bug fixes! Refer to 
[CONTRIBUTING.md](CONTRIBUTING.md) for our contribution requirements.

## License

This service is released under the [MIT License](http://opensource.org/licenses/mit-license.php).
