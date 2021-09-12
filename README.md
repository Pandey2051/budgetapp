# budgetapp
Creating a app that can track our expenses and income.
// Can be used as an identifier, increment each time when you insert a record
let idx = 0; 

/* 
  Please go through the HTML the code first for better understanding
  You don't need to modify HTML to complete this week's task
  No need to worry about the CSS at all
*/

// DOM Selections
const elements = {
  addButton: document.querySelector('.add__btn'),
  selectOption: document.querySelector('.add__type'),
  descBox: document.querySelector('.add__description'),
  budgetValue: document.querySelector('.add__value')
};

// Object to hold the budget records
const budgetRecords = {
  incomes: [], // object structure would be { id, description, value }
  expenses: [],
  incomeTotal: 0,
  expenseTotal: 0,
  remainingBudget: 0,

  addExpense: function (desc, value) {
    // add your code here
    // it should push a new object in the 'this.incomes' array
    this.incomes.push({desc:Salary,value:5000})

  },

  addIncome: function (desc, value) {
    // add your code here
    // it should push a new object in the 'this.expenses' array
    this.expenses.push({desc:rent,value:2000});
  },

  calculateTotal: function () {
    // add your code here
    // find out the values for this.incomeTotal, this.expenseTotal and this.remainingBudget
    this.incomeTotal = incomes[1];
    this.expensesTotal = expenses[1];
    this.remainingBudget = incomeTotal - expensesTotal;

  }
};

// Adds the event listener on the check button
// Everything is done in this part, no need to modify. Just try to understand
elements.addButton.addEventListener('click', () => {
  const recordType = elements.selectOption.value;
  const desc = elements.descBox.value;
  const value = elements.budgetValue.value;

  if (recordType === 'inc') {
    budgetRecords.addIncome(desc, value);
  } else {
    budgetRecords.addExpense(desc, value);
  }

  // shows the object in the console
  console.log(budgetRecords);
});

