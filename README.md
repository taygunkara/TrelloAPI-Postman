# Trello API Testing with Postman & Newman

[Trello API Documentation](https://developer.atlassian.com/cloud/trello/rest/api-group-actions/)

## Tasks:

- Create Board
- Create List
- Update List
- Create Card
- Update Card
- Create Checklist
- Update Checklist
- Create Checkitem
- Create Label
- Update Label
- Delete Label
- Delete Checkitem
- Delete Checklist
- Delete Card
- Get Board
- Delete Board

Test to status codes, names and variables.


## Dependencies
- `npm`, `nodejs`, `newman`, `jenkins(optional)`
---

## Usage

1. Download json file and run this command.
	
```
newman run TrelloAPI-Postman.postman_collection.json \
--environment "https://api.getpostman.com/environments/17544637-27664ee0-f3f1-4762-af23-8beab9147dd1?apikey=PMAK-620a3a66fe1d312ff0b26b69-85aef6fd300fb8dfddd18ea2a90db93a48"

```

or

2. Run this command in your shell.

```
newman run "https://api.getpostman.com/collections/17544637-ae9537e0-1685-4086-a2bf-17a840ac8722?apikey=PMAK-620a3a66fe1d312ff0b26b69-85aef6fd300fb8dfddd18ea2a90db93a48" \
--environment "https://api.getpostman.com/environments/17544637-27664ee0-f3f1-4762-af23-8beab9147dd1?apikey=PMAK-620a3a66fe1d312ff0b26b69-85aef6fd300fb8dfddd18ea2a90db93a48"

```

or

3. Integrate with Jenkins and create junit report.
	
```
newman run "https://api.getpostman.com/collections/17544637-ae9537e0-1685-4086-a2bf-17a840ac8722?apikey=PMAK-620a3a66fe1d312ff0b26b69-85aef6fd300fb8dfddd18ea2a90db93a48" \
--environment "https://api.getpostman.com/environments/17544637-27664ee0-f3f1-4762-af23-8beab9147dd1?apikey=PMAK-620a3a66fe1d312ff0b26b69-85aef6fd300fb8dfddd18ea2a90db93a48" \
-r cli,junit \
--reporter-junit-export "newman/trello.xml"
```
 



