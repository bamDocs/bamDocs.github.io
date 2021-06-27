```plantuml
@startuml
scale 800 width
state "**Part 1: Getting Shampoo Out of Your Eyes With Water**" as Part1 {
  state "1. Calm down" as state1
  state1 : * Pain can lead to panic.
  state1 : * Inhale for 5s
  state1 : * Exhale for 5s
  state1 : * Repeat 3 times

  note left of state1
    Envision yourself
    on a mountaintop
  end note

  state "2. Don't rub your eyes" as state2
  state2: sodium lauryl sulfate
  state2: hurts a lot


  state "3. Close your eyes" as state3
  state3 : Bring your top and
  state3 : bottom eyelids together
  state3 : to close them.

  note left of state3
    Rinse the rest  of
    the shampoo off
  end note

  state "4. Flush your eyes" as state4
  state4: Wash your eyes for 2-3
  state4: minutes
  state4: * Open your eyes
  state4: * Turn your face up


  state "5. Try to cry" as state5
  state5: * optional
  state5: * think of tragic thoughts

  state "6. See a doctor" as state6
  state6: * if you're in pain
  state6: * if your eye is bleeding

  note left of state5
    Imagine you're a
    child alone in the
    woods
  end note

  state1 -> state2
  state1 -[hidden]-> state4
  state2 -> state3
  state3 -> state4
  state3 -[hidden]> state6
  state4 --> state5
  state5 -> state6
}

state "**Part 2: Avoiding Shampoo in Your Eyes**" as Part2 {
  state "1. Tilt your head" as state7
  state7 : look forward at a
  state7:  45 degreeangle

  state "2. Keep eyes closed" as state8
  state8: 1. Get shampoo
  state8: 2. close your eyes
  state8: 3. apply shampoo

  note right of state8
    Not as hard as
    you think
  end note

  state "3. Read the label" as state9
  state9: Directions on the back
  state9: Heed these guidelines
  state9: when utilizing shampoo

  state "4. Don't rub eyes" as state10
  state10: Don't rub your eyes after
  state10: shampooing.

  state "5. Wash your hands" as state11
  state11: * after shampooing
  state11: * soap optional

  state "6. Wear eye protection" as state12
  state12: wear goggles intended for
  state12: acquatic activity

  note right of state12
   can be purchased at
   local sporting goods
   store
  end note

  state "7. Tears-free shampoo" as state13
  state13: * look for pH value of 7


  state "8. Use an eye shield" as state14
  state14: prevents shampoo from
  state14: getting in your eyes

  note right of state14
  goes on your head
  end note

  state7 -> state8
  state7 -[hidden]> state10
  state8 --> state9
  state9 -> state10
  state9 -[hidden]> state12
  state10 --> state11
  state11 -> state12
  state11 -[hidden]> state14
  state12 --> state13
  state13 -> state14
}

Part1 -[hidden]-> Part2

@enduml
