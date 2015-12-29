DataEvents
==========

    Events          |       Handler

    data.load       ->      dataLoading
    data.loaded     ->      dataLoaded
    data.error      ->      dataError
    data.sort       ->      dataSortStart
    data.sorted     ->      dataSortFinish
    data.filter     ->      dataFilterStart
    data.filtered   ->      dataFilterFinish
    data.page.next  ->      dataPageNext
    data.page.prev  ->      dataPagePrev

    item.select     ->      itemSelected
    item.delete     ->      itemDeleted
    item.update     ->      itemUpdated
    item.added      ->      itemAdded

Example header Column Array Object
----------------------------------
    { 
        title: "Id", // the Column Title
        type: "number", // Supported Values are "text" "image" "html" "number"
        sortable: false, // Supported Values are false (disabled) , "both", "ASC", "DESC"
        filterable: false // Bool Enables/Disables Filtering on the Column.
        field: "id" // The Key for the Array for the Data
    }

Example Items Array Object
--------------------------
   {
       "isSelected": false, // (Optional) If its not there it will be added by the table, it's used for the checkboxs
       "id": 32 // the index must be the same as the field in the header
   }