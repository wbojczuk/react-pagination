# react-pagination

<h3>Example of usage</h3>

import Pagination from "./Pagination.jsx";

#THIS IS NEEDED, IT ALLOWS THE COMPONENT TO OUTPUT THE ITEMS ON EACH PAGE
const [pagedItems, setPagedItems] = React.useState("");

function App(){
  return(
  <div>
    {pagedItems}
  </div>
  
  <Pagination
    reload={//SOME STATE TO TRIGGER RELOAD OF PAGINATOR}
    items={allComponents}
    setPagedItems={setPagedItems}
    
    showAmt={4} //Amount of pages to show per view
    itemsPerPage={4} //How Many items to return back per page
   /> 
  )
}
