# DAML_Projects
 
 # 1. UTXO_Token
 a. This token has been designed using the UTXO model. The token transfer process involves two templates i.e. the Token template and the IouTransfer template.

 b. The Token template comprises the Iou_Split and Iou_Merge choices for splitting and merging Token contracts respectively.

 c. Token transfer is implemented via exercising the Iou_Transfer choice in the Token template. This will result in the creation of an IouTransfer contract that is based on the IouTransfer template.

 d. Upon exercising the IouTransfer_Accept choice in the IouTransfer template, a new Token contract will be created with the Token recipient as its new owner and the Token contract of the previous owner is archived.

 e. Test cases are available. In the UTXO_Token.daml file, find the line where "test_setup" is and click on the "Script results" to run the test cases.
