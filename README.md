<table>
  <thead>
    <tr>
      <td><i>features</i></td>
      <th>PostgreSQL</td>
      <th>Riak</th>
      <th>HBase</th>
      <th>MongoDB</th>
      <th>CouchDB</th>
      <th>Neo4j</th>
      <th>Redis</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td class="feature"><b>type of database</b></td>
      <td class="postgresql">Relational</td>
      <td class="riak">Key-Value</td>
      <td class="hbase">Column-Oriented</td>
      <td class="mongodb">answer</td>
      <td class="couchdb">answer</td>
      <td class="neo4j">answer</td>
      <td class="redis">answer</td>
    </tr>
    <tr>
      <td class="feature">
        <b>ACID-compliant</b><br />
        <small>Atomicity, Consistency, Isolation, Durability</small>
      </td>
      <td class="postgresql">Yes</td>
      <td class="riak">No</td>
      <td class="hbase">No</td>
      <td class="mongodb">answer</td>
      <td class="couchdb">answer</td>
      <td class="neo4j">answer</td>
      <td class="redis">answer</td>
    </tr>
    <tr>
      <td class="feature">
        <b>Robust Ad-Hoc Query</b><br />
        <small>Extensive ad-hoc query support means being able to create "on the fly" queries. Opposite of this are "stored procedure" queries.</small>
      </td>
      <td class="postgresql">Yes</td>
      <td class="riak">No</td>
      <td class="hbase">No</td>
      <td class="mongodb">answer</td>
      <td class="couchdb">answer</td>
      <td class="neo4j">answer</td>
      <td class="redis">answer</td>
    </tr>
    <tr>
      <td class="feature">
        <b>Transactions</b><br />
        <small>Unit of work that either succeeds or fails as a whole.</small>
      </td>
      <td class="postgresql">Yes</td>
      <td class="riak">No</td>
      <td class="hbase">No</td>
      <td class="mongodb">answer</td>
      <td class="couchdb">answer</td>
      <td class="neo4j">answer</td>
      <td class="redis">answer</td>
    </tr>
    <tr>
      <td class="feature">
        <b>Scaling</b><br />
        <small>Scaling OUT means multiple parallel datastores rather than a single beefy machine.</small>
      </td>
      <td class="postgresql">Up</td>
      <td class="riak">Out</td>
      <td class="hbase">Out</td>
      <td class="mongodb">answer</td>
      <td class="couchdb">answer</td>
      <td class="neo4j">answer</td>
      <td class="redis">answer</td>
    </tr>
    <tr>
      <td class="feature">
        <b>Fault Tolerant</b><br />
        <small>Servers can go up or down at any moment with no single point of failure.</small>
      </td>
      <td class="postgresql">No</td>
      <td class="riak">Yes</td>
      <td class="hbase">Yes</td>
      <td class="mongodb">answer</td>
      <td class="couchdb">answer</td>
      <td class="neo4j">answer</td>
      <td class="redis">answer</td>
    </tr>
    <tr>
      <td class="feature">
        <b>Schema</b><br />
        <small></small>
      </td>
      <td class="postgresql">Yes</td>
      <td class="riak">No</td>
      <td class="hbase">No</td>
      <td class="mongodb">answer</td>
      <td class="couchdb">answer</td>
      <td class="neo4j">answer</td>
      <td class="redis">answer</td>
    </tr>
    <tr>
      <td class="feature">
        <b>REST Interface</b><br />
        <small>Ability to make CRUD (and other) operations over HTTP API calls.</small>
      </td>
      <td class="postgresql">No</td>
      <td class="riak">Yes</td>
      <td class="hbase">Yes</td>
      <td class="mongodb">answer</td>
      <td class="couchdb">answer</td>
      <td class="neo4j">answer</td>
      <td class="redis">answer</td>
    </tr>
    <tr>
      <td class="feature"><b>Strengths</b></td>
      <td class="postgresql">
        <ul>
          <li>Years of research</li>
          <li>Flexible querability</li>
          <li>Consistent data</li>
        </ul>
      </td>
      <td class="riak">
        <ul>
          <li>High availability</li>
          <li>No single point of failure</li>
          <li>Huge scale</li>
        </ul>
      </td>
      <td class="hbase">
        <ul>
          <li>Made for big jobs</li>
          <li>Built-in versioning</li>
        </ul>
      </td>
      <td class="mongodb">answer</td>
      <td class="couchdb">answer</td>
      <td class="neo4j">answer</td>
      <td class="redis">answer</td>
    </tr>
    <tr>
      <td class="feature"><b>Weaknesses</b></td>
      <td class="postgresql">
        <ul>
          <li>Stiff schema requirements</li>
          <li>Scalability</li>
        </ul>
      </td>
      <td class="riak">
        <ul>
          <li>No ad-hoc query</li>
          <li>Limitations using JavaScript</li>
        </ul>
      </td>
      <td class="hbase">
        <ul>
          <li>Doesn't scale down</li>
          <li>No indexing (other than row keys)</li>
        </ul>
      </td>
      <td class="mongodb">answer</td>
      <td class="couchdb">answer</td>
      <td class="neo4j">answer</td>
      <td class="redis">answer</td>
    </tr>
  </tbody>
</table>

<!-- template
<tr>
  <td class="feature"><b>type</b></td>
  <td class="postgresql">answer</td>
  <td class="riak">answer</td>
  <td class="hbase">answer</td>
  <td class="mongodb">answer</td>
  <td class="couchdb">answer</td>
  <td class="neo4j">answer</td>
  <td class="redis">answer</td>
</tr>
-->
# Glossary

## ACID

* _Atomicity_: an operation is atomic if it either completes entirely or not at all
* _Consistency_: all actions cause the table to transition from one valid state directly to another (eg a row will not disappear during an update, etc)
* _Isolation_: an operation is isolated if it appears to complete independently of any other concurrent transaction
* _Durability_: any update that reports "successful" to the client will not be lost
* _Visibility_: an update is considered visible if any subsequent read will see the update as having been committed

[Source](http://hbase.apache.org/acid-semantics.html)