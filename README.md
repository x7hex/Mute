$nomention 

$onlyIf[$guildID!=;]

$giveRole[$mentioned[1];MUTE_ROLE_ID]

$onlyBotPerms[manageroles;`❌` I need manage roles permission to mute someone!]

$onlyPerms[manageroles;`❌` You don’t have enough permissions to use this command!]

$onlyIf[$rolePosition[$highestRole[$authorID]]<$rolePosition[$highestRole[$mentioned[1]]];> `❌` This user has a higher role position than you!]

$onlyIf[$rolePosition[$highestRole[$botID]]<$rolePosition[$highestRole[$mentioned[1]]];> `❌` This user has a higher role position than me!]

$author[$username[$mentioned[1]]#$discriminator[$mentioned[1]] Was Muted!] 

$authorIcon[$userAvatar[$mentioned[1]]

$description[`🤬` Reasoning: $replaceText[$replaceText[$checkCondition[$message[2]==];true;No reason.;1];false;$replaceText[$message;$message[1];;1];1]
`🔧` Moderator: <@$authorID>
`⏰` Time: <t:$getTimestamp>]

$color[#36393F]

$endif
