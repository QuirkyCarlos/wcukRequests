If you have any questions please contact us at Discord.com 
https://discord.gg/GZnFrxRnRK

Future updates and plans will also be available on discord

# To display a request

[Server side] 
TriggerClientEvent("wcukRequests:RequestMenu", source, target, time, title, message, trigger, side, parameters, parametersNum) 

[Client side]
exports['wcukRequests']:requestMenu(target, time, title, message, trigger, side, parameters, parametersNum)

	The target field defines who receives the request.
	The time field lets you set the time the request window will stay on the screen.
	The title field is where you set the title of the request.
	The message field lets you choose the message that will appear on the request window.
	The trigger field is where you choose the event that will be executed.
	The side (client/server) field allows you to choose if the trigger is client or server sided.
	The parameters field contains the parameters the trigger takes.
	The parametersNum field are the number of paramenters used.

# Example
TriggerClientEvent("wcukRequests:RequestMenu", source, tonumber(args[1]), 10000, "<i class='fas fa-question-circle'></i>&nbsp;Job Offer", "Tommy wants to hire you.", "client", "parameter1,parameter2,parameter3,parameter4,parameter5", 5)

	The 'side' field should be either 'client' or 'server'.
	The 'parameters' field needs to be a string, all parameters need to be seperated by a comma ',' without any spaces!
	Do not forget to set the number of parameters used, in the 'parametersNum' field.
	And if you don't have any parameters you don't need to add the 'parameters' and the 'parametersNum' field.

[Dark/Light Theme]

	To enable/disabled the dark/light mode you should open scripts.js and navigate to the line 1.
	If the 'var darkMode' is set to true, the dark theme will be enabled, otherwise it will enable the light mode.