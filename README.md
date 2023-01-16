### Features

- Keeps all logic behind the frontend (the navigator), working as a backend fully functional
- Detects when the amount of money requested is superior or not in comparison to the cash that the ATM has avaliable
- Displays the number of the money requested, as well as the pictures of each bill it will require for such amount

# ATM-Django



                
###User Flux 

```flow
st=>start: Start
ns=>operation: Number selection
conf=>condition: Confirmation
cond=>condition: Enough cash?
goodend=>end: Money Requested

st->ns->conf
conf(yes)->cond
conf(no)->ns
cond(yes)->goodend
cond(no)->ns

```

###End
