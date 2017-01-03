# Manifesto

McValidator implementin' manifesto. Keeping data validation easy as shoottin' fish in a barrel.

## Validator

Validator will validate(ain't no shit sherlock) the plumbing flow with __Rules__, if some anomaly found on the flow, validator can stop the validation and throw some error, or just return false.

## Rules

Rules will control the flow validation, ruling the data and not letting a single dirty thing pass through the pipe.

## Regulator

Regulators works aside of __Rules__ to ensure the data existence.

## Filters

Filters will ensure that the data will always be the same, when someone send `"123"` on your API, you can ensure that the backend will always receive `123` as integer, not as string, not as long, not as float, not as decimal, but as integer. Filters can also join multiple fields into 1, or split 1 field into multiples fields. __Rules__ can use __Filters__ to always receive a valid input besides its validation, yeah, we life things safe.

## Plumbing

We do like plumbers and also plumbing(and mudkipz), *McValidor* will keep it structure of __Filters__ and __Rules__ into a pipe structure, __Filters__ will be run first, then __Rules__ will run. If you need validate __Filter__ input first, __Filter__ has its own rules. You can append and preprend things into the plumbing with __Joints__

## Joints

Joints store __Rules__ and __Regulators__, each field on the input have its own __Joint__.

## Value

Value store value and its __Filter__ and __Rule__ history, so, you can know the path where your data has pass.

[Imgur](http://i.imgur.com/pZds4dh.png)
