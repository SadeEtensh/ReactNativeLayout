# React Native Layout

## `For anyOne Aspiring to be React Native Developer`

## Important Points

- To work with Layout we have Flexbox in React native
  -Flexbox contain of 2 main entities

1. Flex container
2. flex items

- Axes in React Native:

1. Main axis--> run from `Top' to #bottom
2. Cross axis--> runs from #Left to #Right
   ![Alt text](<Screenshot 2023-10-15 at 9.37.47 at night.png>)

## flex

- The flex property plays a crucial role in defining how much of view will fill the screen along main axis.
- It accepts an Integer value greater than or equals to 0, indicating the fraction of the available space that the component should occupy.
- The View container in React Native has already display: flex set by defualt-the property that changes div to flex container.
- The flex property is NOT limited to container but its also applicable to flex items (takes fraction of available space).

## flexDirection

- The flexDirection property establishes the `main axis`, which in turn determins how the flex items are placed within container.
- By default, the main axis flows from Top to bottom, causing the items to be displayed from top to bottom in the UI.
- However, by chaning the value of `flexDirection` property, we can alter how the items are positioned. it has 4 diffrent values

## justifyContent

- defines the aligiment along the `main axis`
- setted on container to align items

  ### possible values

- `flex-start` ---> the default Value.
- `flex-end` ---> causes flex items to be placed at the `End` of main axis
- `center` --> places flex items at the center of main axis
- `space-between`---> distributes `spaces` between items
- `space-arround` --> In this case, space at the beggining/end is `half(1/2) ` of space between flex items
- `space-evenly` ---> equal space distribution on all flex items

`Note`: justifyContent(jC) is dependant on `main axis`

- if flexDirection value is `row` it also changes the main axis LTR

## AlignItems

- defines the default behavior for laying out flex itemsa along the container's `Cross axis`.
- Works similar with justifyContent but in the perpendicular direction
  ### Posible values
- `stretch` --> is default Value, meaning the flex items stretch the entire length of cross axis in LTR.
- `flex-start`--> pushes the flex items to the `start` of cross axis
- `flex-end`--> pushes the flex items to the `end` of the cross axis
- `center` --> centers the content on cross axis.
- `baseline` --> align elements based on their contents baseline.

## alignSelf

- Unlike `alignItems` which is applied to the container and controls the alignment of all items within it.
- `alignSelf` is applied to individual items, allowing us to control the alignment of each items independantly.
- The values available for alignSelf is similar to those used in `alignItems`

- Note: the default value of `alignSelf` not stretch but it is `auto` meanining it inherits its value from the `alignitems` property of its parent flex container.

![Alt text](<Screenshot 2023-10-16 at 4.27.10 in the afternoon.png>)
