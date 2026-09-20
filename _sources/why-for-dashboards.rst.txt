Why a Cloud Fits Interactive Dashboards
=======================================

A Plotly Dash app is a **long-running web process**. It runs continuously
and talks back and forth with every browser that touches it — sliders,
callbacks, filters. A dashboard therefore needs three things: a machine that
stays on, a network address the internet can reach, and a place to put your
data. A cloud provides all three in minutes, and each maps directly onto a
Jetstream2 feature.

A machine that stays on
-----------------------

You launch a virtual machine, log in, and install Dash:

.. code-block:: text

   pip install dash
   dash run --port 8050

The process keeps running whether or not anyone is looking at it — exactly
like the lab server you would deploy on-premises, only it lives in a
national cloud.

A URL anyone can open
---------------------

Every VM can have a public IP address, or a free DNS name of the form
``name.ALLOCATION.projects.jetstream-cloud.org``. Anyone with the link can
open your dashboard in a browser — a co-author in another lab, a reviewer, a
student. Your analysis goes from a static figure to something people can
actually *poke at*.

Controlled access
-----------------

Security groups control who can reach the dashboard's port: open it to your
lab's address range, or to the whole world — your choice. When a dashboard
graduates into a real service, you can put automatic HTTPS in front of it
(Caddy + Let's Encrypt) and point your own domain at it with a CNAME record.

A home for your data
--------------------

Datasets live on block storage or in S3-compatible object storage, attached
to your VM the same way a local disk would be. And when you are done for the
day you can **shelve** the VM: a shelved machine costs nothing, so an
allocation stretches much further than its nominal size suggests.
