
[![Alphalake.ai](https://www.alphalake.ai/hs-fs/hubfs/AL_BLUE-4.png?width=1660&name=AL_BLUE-4.png)](https://www.alphalake.ai/)

# Workato Connector: Robocorp
Connect to Workato IPaaS with Robocorp. This Workato connector provides support for Robocorp in order to:

 - Call a Robocorp robot/process to run from within Workato
 - Get the output from a given robot/process run

## Requirements

 - Workato API Key
 - Robocorp control room API Key
 - Robocorp workspace ID
 - Some actions will also require the Workspace ID, Process ID, Robot ID, Work item ID, Process run ID
## Actions
####  Create a new Robot
	 This action will create a new work item as an input in the given process.
#### Get a link to upload a robot
	This action will output a link to upload a robot to the given control room.
#### Get a link to download a robot
	This action will output a link to download the robot with the given robot ID.
#### Get process work item
	This action will get the specified work item and will need the Workspace ID, Process ID and work item ID.
#### Get robot run
	This will fetch the specified run of a robot and return the start/end time, status, step, duration, and 
	result of the run.
#### Get robot run artifact
	This will get the robot run artifact of a process run.
#### Get work item file download link
	This action will output a download link to the specified work item.
#### List process run work items
	This will list all of the work items from the specified process run.
#### List process runs in process
	This will output all the process runs from a given process.
#### List process runs in workspace
	This will output all the process runs in the given workspace.
#### List process work items
	This action will output all of the work items from a given process.
#### List processes
	This will output a list of all the processes in a given workspace
#### List robot run artifacts
	This will output a list of all the run artifacts from a specified process run.
#### List robot run console messages
	This will output a list of the console messages from a specified run.
#### List robot run events
	This action will output a list of the robot run events from a given process run.
#### List robot runs
	This action will list the robot runs from the given process.
#### Mark work item as completed
	Marks a work item as completed. This will cause the work item to be set to the completed state 
	and it will not be processed further. Operation can only be performed on work items in the state Failed.
#### Monitor process run status
	This action will monitor the process run status and will return if the run is in progress, complete or 
	failed.
#### Register work item file upload
	Registers a new work item file and returns file upload info. The output is a JSON object declaring the
	URL and form fields that can be used to actually POST the binary file.
#### Retry processing of work item
	Requests reprocessing of a work item. Work item is then processed again in the same process run and 
	process step. Operation can only be performed on work items in state Failed.
#### Start a process with an optional work item payload
	Starts a process run with a new work item. If the request has a body, the body is used as a data payload
	for a new work item. The payload must be a valid JSON (RFC 7159). Even if the body is an array, it is
	interpreted as a single payload (in this case an array object). If the request has no body, a new work item
	is created without a payload.
#### Starts a process with multiple work items
	The request body is expected to contain multiple work item data payloadsd. The body must be a validd JSON
	array (RFC 7159). A new work item is created for each payload (element in the deserialised array).
#### Starts a process with provided configuration, by the following rules
	If type = default: the process is started based on process default configuration. No parameters.
	If type = workItemIDs: the process is started with given work items. Additional parameter WorkItemIDs
	required
#### Update work item data (JSON)
	Overwrites the work item data (JSON) payload.
## Robocorp Connector video
[![Alphalake.ai](https://www.alphalake.ai/hubfs/graphic.png)](https://www.alphalake.ai/robocorp-connector)
