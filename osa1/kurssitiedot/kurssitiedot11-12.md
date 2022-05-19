Laitan nämä tiedostot nyt näin, laitan lopussa sitten koko ohjelman lähdekoodi

const exercise1 = 10
const exercise2 = 7
const exercise3 = 14
const part1 = 'Fundamentals of React'
const part2 = 'Using props to pass data'
const part3 = 'State of a component' 

const Header = (props) => {
  return (
    <h1>{props.course}</h1>
  )
}

const Content = (props) => { 
  
  return (
    <div>
      <p>{props.part1} {props.exercise1}</p>
      <p>{props.part2} {props.exercise2}</p>
      <p>{props.part3} {props.exercise3}</p>
      
    </div>
  )
}

const Total = (props) => {
  return (
    <p>{props.name} {exercise1 + exercise2 + exercise3}</p>
  )
}

const App = () => {

  const course = 'Half Stack application development'
 
  const total = 'Number of exercises'

  return (

    <div>

      <Header course={course}/>
      <Content part1={part1} exercise1={exercise1}
      part2={part2} exercise2={exercise2}
      part3={part3} exercise3={exercise3} />
      <Total name = {total}/> 
    
    </div>
          )
  }

export default App