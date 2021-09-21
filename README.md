frappe.ui.form.on('GPAN Portal Platform Individual1', {
          validate:  function(frm) {
        	// make calculation on the fields  
           var a = frm.doc.price + frm.doc.monthly_contributions;

    		frm.set_value("total_usd_contribution", a);
    		frm.refresh_field("total_usd_contribution");

    		var b = frm.doc.monthly + frm.doc.monthly_contributions;
    		frm.set_value("grand_crowning", b);
    		frm.refresh_field("grand_crowning");



        }
    });
