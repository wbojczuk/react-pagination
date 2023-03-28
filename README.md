# react-pagination

<h3>Example of usage</h3>

    import Pagination from "./Pagination.jsx";
    
    const [reloadPage, setReloadPage] = React.useState("");
    const [pagedItems, setPagedItems] = React.useState("");
    const allComponents = [<div></div>,<div></div>,<div></div>,<div></div>,<div></div>,<div></div>];

    function App(){
      return(
      
      <div>
        // Output the returned Items here
        {pagedItems}
      </div>

      <Pagination
        reload={reloadPage}
        items={allComponents}
        setPagedItems={setPagedItems}
        showAmt={4}
        itemsPerPage={4}
       /> 
       
      )
    }

&bull; reload - In case you're working with a SPA, or such. You want the Paginator to reload when a new page/view is rendered. To accomplish this, include a React.state here and change it when a reload is needed.<br><br>

&bull; items - These are the components that you want to break down into pages, takes an array. Exactly what you put in is what you get back<br><br>

&bull; setPagedItems - This is the State set function for the elements you will be recieving back. You will use the corresponding value (pagedItems) to output that specific page's components. Check the above code for an example<br><br>

&bull; showAmt -  This determines the amount of pages visible between the arrows (if applicable).<br><br>

&bull; itemsPerPage - The amount of items to return before making new page<br><br>
