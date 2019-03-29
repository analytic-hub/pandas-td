# Version History

## 0.10.0 (2019-03-29)

* Set minimum requests version to 2.21.0 (#9)

## 0.9.0 (2018-08-31)

* Tweaked dependency versions (#7, #8)

## 0.8.8 (2015-12-13)

* New magic function %td_job.
* New option --timezone (-T) for magic query functions.
* New option --connection (-c) for magic query functions.
* Deprecated option --engine (-e) for magic query functions.
* (Experimental) New function ``create_queue`` for background job execution.
* (Experimental) New option --queue (-a) for magic query functions.
* Support HipChat and Slack as notification channel for background jobs.

## 0.8.7 (2015-11-23)

* Several bug fixes of to_td().

## 0.8.6 (2015-11-12)

* to_td() now waits until imported data becomes visible.  It also prints progress in HTML.
* New option --engine (-e) for magic query functions.

## 0.8.5 (2015-10-09)

* New function ``read_td_job``.

## 0.8.4 (2015-08-07)

* New option --out-file (-O) for magic query functions.
* Magic query functions --plot and --pivot options regard "_id" as dimensions.

## 0.8.3 (2015-07-27)

* Add 'clear_progress' parameter to create_engine.
* Magic query functions now substitute variables into query text.
* New option --dry-run for magic query functions.

## 0.8.2 (2015-07-20)

* Minor bug fixes.

## 0.8.1 (2015-07-18)

* Add options for ``%%td_hive``, ``%%td_pig``, and ``%%td_presto``.
* ``%%td_hive_plot``, ``%%td_pig_plot``, and ``%%td_presto_plot`` are deprecated.  Use ``--plot`` options instead.

## 0.8.0 (2015-07-13)

* New function ``create_engine``.
* (Experimental) New module ``pandas_td.ipython`` for magic functions.
* ``Connection.databases`` and ``Connection.tables`` are deprecated.  Use magic functions.
* ``Connection.query_engine`` is deprecated.  Use ``create_engine`` instead.
* ``read_td_query`` sets ``distributed_join = 'false'`` by default for Presto.
