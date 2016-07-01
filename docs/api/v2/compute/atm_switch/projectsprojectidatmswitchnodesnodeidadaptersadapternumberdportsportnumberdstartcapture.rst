/v2/compute/projects/{project_id}/atm_switch/nodes/{node_id}/adapters/{adapter_number:\d+}/ports/{port_number:\d+}/start_capture
------------------------------------------------------------------------------------------------------------------------------------------

.. contents::

POST /v2/compute/projects/**{project_id}**/atm_switch/nodes/**{node_id}**/adapters/**{adapter_number:\d+}**/ports/**{port_number:\d+}**/start_capture
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Start a packet capture on an ATM switch instance

Parameters
**********
- **adapter_number**: Adapter on the switch (always 0)
- **project_id**: Project UUID
- **port_number**: Port on the switch
- **node_id**: Node UUID

Response status codes
**********************
- **200**: Capture started
- **400**: Invalid request
- **404**: Instance doesn't exist

Input
*******
.. raw:: html

    <table>
    <tr>                 <th>Name</th>                 <th>Mandatory</th>                 <th>Type</th>                 <th>Description</th>                 </tr>
    <tr><td>capture_file_name</td>                    <td>&#10004;</td>                     <td>string</td>                     <td>Capture file name</td>                     </tr>
    <tr><td>data_link_type</td>                    <td> </td>                     <td>enum</td>                     <td>Possible values: DLT_ATM_RFC1483, DLT_EN10MB, DLT_FRELAY, DLT_C_HDLC</td>                     </tr>
    </table>
