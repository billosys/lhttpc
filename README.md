# lhttpc

## ESL Notice

This project is no longer supported by Erlang Solutions. Instead, they recommend using [shotgun](https://github.com/inaka/shotgun) or [fusco](https://github.com/esl/fusco).


## BilloSystems Noice

We actually really like lhttpc and are happy with it. We'll maintain a repo for it until we run into limitations
(we haven't so far).


## Building

For versions > 1.2.5, lhttpc is built using [rebar](https://github.com/rebar/rebar). There is still a ``Makefile`` with some of the old make targets, such as all, doc, test etc. for those who prefer that. The ``Makefile`` will however just call rebar.


## ``ENV`` Configuration

 * ``connection_timeout``: The time (in milliseconds) the client will try to
                           kepp a HTTP/1.1 connection open. Changing this value
                           in runtime has no effect, this can however be done
                           through ``lhttpc_manager:update_connection_timeout/1``.
