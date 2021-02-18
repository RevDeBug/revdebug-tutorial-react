# REVDEBUG REACT TUTORIAL

Simple React example, click the "CRASH" button to crash. No I don't know why the top level unhandled exception is triggered twice, it happens in the browser and is recorded that way accurately.

Configure RevDeBug repository:

    npm config set @revdebug:registry https://nexus.revdebug.com/repository/npm/

Install dependancies (including RevDeBug):

    npm install

\* Note: Before instrumenting you may need to change the "host" (and maybe "port" / "webPort") fields in "revdebug.json" or specify different values on the command line if you are not running the record server locally.

Normal instrument:

    npx revd

Or instrument passing different host:

    npx revd --host your_record_server.com

And off we go...

    npm start

Click the "CRASH" button then have a look at the crash recording in devops monitor.
