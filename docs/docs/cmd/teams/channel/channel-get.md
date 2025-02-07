# teams channel get

Gets information about the specific Microsoft Teams team channel

## Usage

```sh
m365 teams channel get [options]
```

## Options

`-i, --teamId [teamId]`
: The ID of the team to which the channel belongs to. Specify either teamId or teamName but not both

`--teamName [teamName]`
: The display name of the team to which the channel belongs to. Specify either teamId or teamName but not both

`-c, --id [id]`
: The ID of the channel for which to retrieve more information. Specify either id or name but not both

`--name [name]`
: The display name of the channel for which to retrieve more information. Specify either id or name but not both

`--primary`
: Gets the default channel, General, of a team. If specified, id or name are not needed

--8<-- "docs/cmd/_global.md"

## Examples
  
Get information about Microsoft Teams team channel with id _19:493665404ebd4a18adb8a980a31b4986@thread.skype_

```sh
m365 teams channel get --teamId 00000000-0000-0000-0000-000000000000 --id '19:493665404ebd4a18adb8a980a31b4986@thread.skype'
```

Get information about Microsoft Teams team channel with name _Channel Name_

```sh
m365 teams channel get --teamName "Team Name" --name "Channel Name"
```

Get information about Microsoft Teams team primary channel , i.e. General

```sh
m365 teams channel get --teamName "Team Name" --primary
```
