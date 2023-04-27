# Property Rentals
Apply for renting a property for a specific term and get rejected or approved by the superintendent.

### I. Workflow
1. A renter creates a RentalApplication contract. Both renter and superintendent are invited as observers, but superintendent, as a controller, is authorized to exercise either Reject or Accept on the RentalApplication.
2. Upon the controller exercising Reject, a new contract is created to give the chance to the renter to bump the amount offered increasing the chance in getting accepted.
3. Revise choice can be exercised on the newly generated contract from above.
4. Accept choice is exercised to finalize the rental application and generate a new RentalAgreement contract.

[![Demo](./Demo.png)](https://share.vidyard.com/watch/xbDuZMbNUbgfHmPnqzt72N?)

### II. Building
To compile the project
```
$ daml build
```

### III. Testing
To test all scripts:
Either run the pre-written script in the `Test.daml` under /daml OR run:
```
$ daml test
```

### IV. Running
To load the project into the sandbox and start navigator:
```
$ daml start
```
