## information search happy path
* greet
  - utter_greet
* mood_great
  - utter_ask_name
* name_data{"name":"Sarika"}
  - utter_ask_location
* search_provider{"location":"Hyderabad"}
  - utter_ask_occupation
* inform{"occupation":"doctor"}
  - utter_ack
* thanks
  - utter_goodbye

## information search + location
* greet
  - utter_greet
* mood_great
  - utter_ask_name
* name_data{"name":"Sarika"}
  - utter_ask_location
* search_provider{"location":"Hyderabad"}
  - utter_ask_occupation
* inform{"occupation":"doctor"}
  - utter_ack
* thanks
  - utter_goodbye
  
## happy path
* greet
  - utter_greet
* mood_great
  - utter_happy
* thanks
  - utter_goodbye

## sad path 1
* greet
  - utter_greet
* mood_unhappy
  - utter_cheer_up
  - utter_did_that_help
* affirm
  - utter_happy

## sad path 2
* greet
  - utter_greet
* mood_unhappy
  - utter_cheer_up
  - utter_did_that_help
* deny
  - utter_goodbye

## say goodbye
* goodbye
  - utter_goodbye

## bot challenge
* bot_challenge
  - utter_iamabot
