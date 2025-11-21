# Unreal's Duplication

In Unreal Engine's PIE or Sequence Render mode, it performs a world copy operation.

<img src="./Images/Unreal's Duplication/PIEDuplication1.png" alt="PIEDuplication1">

## Time series

Unreal's Dupliacte performs Write Serialize on the source data and Read Serialize on the new data to be copied. Only UProperty or other data involved in serialization will be copied. UProperty marked with Transient will not be copied.

<img src="./Images/Unreal's Duplication/PIEDuplication2.png" alt="PIEDuplication2">

<img src="./Images/Unreal's Duplication/PIEDuplication3.png" alt="PIEDuplication3">

## Some just init once, and join Duplication

You can declare a regular variable and modify it during PostDuplicate.

<img src="./Images/Unreal's Duplication/PIEDuplication4.png" alt="PIEDuplication4">

<img src="./Images/Unreal's Duplication/PIEDuplication5.png" alt="PIEDuplication5">

Then just init it when not duplicate.

<img src="./Images/Unreal's Duplication/PIEDuplication6.png" alt="PIEDuplication6">

<img src="./Images/Unreal's Duplication/PIEDuplication7.png" alt="PIEDuplication7">
