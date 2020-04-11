## General Tour
* greet
  - utter_greet
* tour.general
  - utter_show_filters
  - utter_ask_continue
* tour.general
  - utter_show_search
  - utter_ask_continue
* affirm
  - utter_show_icons
  - utter_ask_continue
* affirm
  - utter_show_catscreen
  - utter_show_suppliers
  - utter_end_tour
* affirm
  - utter_contact_details
  - utter_thanks
* goodbye
  - utter_goodbye

## General Tour Choices
* tour.question{"topic": "updates"}
   - slot{"topic": "updates"}
   - action_tour
   - utter_ask_continue_query

## General Tour Early Exit
* greet
  - utter_greet
* tour.general
  - utter_show_filters
  - utter_ask_continue
* affirm
  - utter_show_search
  - utter_ask_continue
* goodbye
  - utter_goodbye

## General Tour Early Exit 2
* greet
  - utter_greet
* tour.general
  - utter_show_filters
  - utter_ask_continue
* goodbye
  - utter_goodbye

## Supplier Information
* greet
  - utter_greet
* supplier.general
  - utter_supplier_menu

## Feedback
* greet
  - utter_greet
* feedback
  - utter_thanks
  - form_get_rating
  - form{"name": "form_get_rating"}
  - form{"name": null}
  - form_get_influence
  - form{"name": "form_get_influence"}
  - form{"name": null}
  - utter_pre_finish
  - utter_finish

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

## General Tour questions Early Exit1

* greet
    - utter_greet
* tour.general
    - utter_show_filters
    - utter_ask_continue
* tour.question{"topic":"contacts"}
    - slot{"topic":"contacts"}
    - action_tour
    - utter_ask_continue_query
* tour.general
  - utter_show_search
  - utter_ask_continue
* affirm
  - utter_show_icons
  - utter_ask_continue
* affirm
  - utter_show_catscreen
  - utter_show_suppliers
  - utter_end_tour
* affirm
  - utter_contact_details
  - utter_thanks
* goodbye
  - utter_goodbye

## tour into feedback

* greet
    - utter_greet
* tour.general
    - utter_show_filters
    - utter_ask_continue
* tour.question{"topic":"negoroadmap"}
    - slot{"topic":"negoroadmap"}
    - action_tour
    - utter_ask_continue_query
* main_menu
    - utter_main_menu
* feedback
    - utter_thanks
    - form_get_rating
    - form{"name":"form_get_rating"}
    - slot{"requested_slot":"rating"}
* feedback
    - form_get_rating
    - slot{"rating":"3"}
    - form{"name":null}
    - slot{"requested_slot":null}
    - form_get_influence
    - form{"name":"form_get_influence"}
    - form{"name":null}
    - slot{"requested_slot":null}
    - utter_pre_finish
    - utter_finish

## Tour Early Exit into Supplier
* greet
    - utter_greet
* tour.general
    - utter_show_filters
    - utter_ask_continue
* affirm
    - utter_show_search
    - utter_ask_continue
* main_menu
    - utter_main_menu
* supplier.general
    - utter_supplier_menu
* goodbye
    - utter_goodbye

## General Tour questions

* greet
    - utter_greet
* tour.general
    - utter_show_filters
    - utter_ask_continue
* affirm
    - utter_show_search
    - utter_ask_continue
* tour.question{"topic":"contracts"}
    - slot{"topic":"contracts"}
    - action_tour
    - utter_ask_continue_query
* goodbye
    - utter_goodbye

## Tour bad ending

* greet
    - utter_greet
* tour.general
    - utter_show_filters
    - utter_ask_continue
* affirm
    - utter_show_search
    - utter_ask_continue
* affirm
    - utter_show_icons
    - utter_ask_continue
* affirm
    - utter_show_catscreen
    - utter_show_suppliers
    - utter_end_tour
* tour.question{"topic":"strategies"}
    - slot{"topic":"strategies"}
    - action_tour
    - utter_ask_continue_query
* goodbye
    - utter_goodbye

## Category Search Happy

* greet
    - utter_greet
* category.search
    - form_get_category
    - form{"name": "form_get_category"}
    - form{"name": null}
    - action_search
    - utter_did_that_help
* affirm
    - utter_goodbye

## Category Search Unhappy

* greet
    - utter_greet
* category.search
    - form_get_category
    - form{"name": "form_get_category"}
* stop
    - utter_ask_continue
* deny
    - action_deactivate_form
    - form{"name": null}

## Category Search1

* category.search
    - form_get_category
    - form{"name": "form_get_category"}
    - form{"name": null}
    - action_search
    - utter_did_that_help
* affirm
    - utter_goodbye

## faq
* faq
   - respond_faq

## Tour Interrupt FAQ

* greet
    - utter_greet
* tour.general
    - utter_show_filters
    - utter_ask_continue
* affirm
    - utter_show_search
    - utter_ask_continue
* affirm
    - utter_show_icons
    - utter_ask_continue
* faq
    - respond_faq
    - utter_ask_continue
* affirm
    - utter_show_catscreen
    - utter_show_suppliers
    - utter_end_tour
* affirm
    - utter_contact_details
    - utter_thanks

## Tour Interrupt FAQ1

* greet
    - utter_greet
* tour.general
    - utter_show_filters
    - utter_ask_continue
* affirm
    - utter_show_search
    - utter_ask_continue
* faq
    - respond_faq
    - utter_ask_continue
* affirm
    - utter_show_icons
    - utter_ask_continue
* affirm
    - utter_show_catscreen
    - utter_show_suppliers
    - utter_end_tour
* affirm
    - utter_contact_details
    - utter_thanks

## Tour Interrupt FAQ2

* greet
    - utter_greet
* tour.general
    - utter_show_filters
    - utter_ask_continue
* faq
    - respond_faq
    - utter_ask_continue
* affirm
    - utter_show_search
    - utter_ask_continue
* affirm
    - utter_show_icons
    - utter_ask_continue
* affirm
    - utter_show_catscreen
    - utter_show_suppliers
    - utter_end_tour
* affirm
    - utter_contact_details
    - utter_thanks

## Tour_FAQ_Question_CategorySearch

* greet
    - utter_greet
* tour.general
    - utter_show_filters
    - utter_ask_continue
* faq
    - respond_faq
    - utter_ask_continue
* affirm
    - utter_show_search
    - utter_ask_continue
* tour.question
    - action_tour
    - utter_ask_continue_query
* tour.question{"topic":"contracts"}
    - slot{"topic":"contracts"}
    - action_tour
    - slot{"topic":"contracts"}
    - utter_ask_continue_query
    - slot{"topic":"contracts"}
* category.search
    - form_get_category
    - form{"name":"form_get_category"}
    - slot{"requested_slot":"category"}
* category.search{"category":"Infrastructure"}
    - slot{"category":"Infrastructure"}
    - form_get_category
    - slot{"category":"Infrastructure"}
    - form{"name":null}
    - slot{"requested_slot":null}
    - action_search
    - slot{"category":"Infrastructure"}
    - utter_did_that_help
* affirm
    - utter_goodbye
