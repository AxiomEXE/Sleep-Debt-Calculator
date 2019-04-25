# Sleep-Debt-Calculator

```markdown

const getSleepHours = day =>{
  switch (day) {
    case 'Monday':
      return 8;
      break;
    case 'Tuesday':
      return 8;
      break;
    case 'Wednesday':
      return 8;
      break;
    case 'Thursday':
      return 8;
      break;
    case 'Friday':
      return 8;
      break;
    case 'Saturday':
      return 8;
      break;
    case 'Sunday':
      return 8;
      break;
  }
}

const getActualSleepHours = () =>
  getSleepHours('Monday') +
  getSleepHours('Tuesday') +
  getSleepHours('Wednesday') +
  getSleepHours('Thursday') +
  getSleepHours('Friday') +
  getSleepHours('Saturday') +
  getSleepHours('Sunday');

const getIdealSleepHours = () =>{
  const idealHours = 8;
  return idealHours * 7;
}

const calculateSleepDebt = () =>{
  const actualSleepHours = getActualSleepHours();
  const idealSleepHours = getIdealSleepHours();
  if (actualSleepHours == idealSleepHours){
    console.log('You got the perfect amount of sleep!')
  } else if (actualSleepHours >= idealSleepHours){
    console.log(`You only got ${actualSleepHours - idealSleepHours} hours more sleep and don't need as much rest.`)
  } else if (actualSleepHours <= idealSleepHours){
    console.log(`You only got ${idealSleepHours - actualSleepHours} hours less sleep and need to get more rest.`)
  }
}

calculateSleepDebt();

```
