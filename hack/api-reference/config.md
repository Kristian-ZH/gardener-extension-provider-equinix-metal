<p>Packages:</p>
<ul>
<li>
<a href="#equinixmetal.provider.extensions.config.gardener.cloud%2fv1alpha1">equinixmetal.provider.extensions.config.gardener.cloud/v1alpha1</a>
</li>
</ul>
<h2 id="equinixmetal.provider.extensions.config.gardener.cloud/v1alpha1">equinixmetal.provider.extensions.config.gardener.cloud/v1alpha1</h2>
<p>
<p>Package v1alpha1 contains the Equinix Metal provider configuration API resources.</p>
</p>
Resource Types:
<ul></ul>
<h3 id="equinixmetal.provider.extensions.config.gardener.cloud/v1alpha1.ControllerConfiguration">ControllerConfiguration
</h3>
<p>
<p>ControllerConfiguration defines the configuration for the Equinix Metal provider.</p>
</p>
<table>
<thead>
<tr>
<th>Field</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td>
<code>clientConnection</code></br>
<em>
<a href="https://godoc.org/k8s.io/component-base/config/v1alpha1#ClientConnectionConfiguration">
Kubernetes v1alpha1.ClientConnectionConfiguration
</a>
</em>
</td>
<td>
<em>(Optional)</em>
<p>ClientConnection specifies the kubeconfig file and client connection
settings for the proxy server to use when communicating with the apiserver.</p>
</td>
</tr>
<tr>
<td>
<code>etcd</code></br>
<em>
<a href="#equinixmetal.provider.extensions.config.gardener.cloud/v1alpha1.ETCD">
ETCD
</a>
</em>
</td>
<td>
<p>ETCD is the etcd configuration.</p>
</td>
</tr>
<tr>
<td>
<code>healthCheckConfig</code></br>
<em>
<a href="https://github.com/gardener/gardener/extensions/pkg/controller/healthcheck/config">
github.com/gardener/gardener/extensions/pkg/controller/healthcheck/config/v1alpha1.HealthCheckConfig
</a>
</em>
</td>
<td>
<em>(Optional)</em>
<p>HealthCheckConfig is the config for the health check controller</p>
</td>
</tr>
</tbody>
</table>
<h3 id="equinixmetal.provider.extensions.config.gardener.cloud/v1alpha1.ETCD">ETCD
</h3>
<p>
(<em>Appears on:</em>
<a href="#equinixmetal.provider.extensions.config.gardener.cloud/v1alpha1.ControllerConfiguration">ControllerConfiguration</a>)
</p>
<p>
<p>ETCD is an etcd configuration.</p>
</p>
<table>
<thead>
<tr>
<th>Field</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td>
<code>storage</code></br>
<em>
<a href="#equinixmetal.provider.extensions.config.gardener.cloud/v1alpha1.ETCDStorage">
ETCDStorage
</a>
</em>
</td>
<td>
<p>ETCDStorage is the etcd storage configuration.</p>
</td>
</tr>
</tbody>
</table>
<h3 id="equinixmetal.provider.extensions.config.gardener.cloud/v1alpha1.ETCDStorage">ETCDStorage
</h3>
<p>
(<em>Appears on:</em>
<a href="#equinixmetal.provider.extensions.config.gardener.cloud/v1alpha1.ETCD">ETCD</a>)
</p>
<p>
<p>ETCDStorage is an etcd storage configuration.</p>
</p>
<table>
<thead>
<tr>
<th>Field</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td>
<code>className</code></br>
<em>
string
</em>
</td>
<td>
<em>(Optional)</em>
<p>ClassName is the name of the storage class used in etcd-main volume claims.</p>
</td>
</tr>
<tr>
<td>
<code>capacity</code></br>
<em>
<a href="https://godoc.org/k8s.io/apimachinery/pkg/api/resource#Quantity">
k8s.io/apimachinery/pkg/api/resource.Quantity
</a>
</em>
</td>
<td>
<em>(Optional)</em>
<p>Capacity is the storage capacity used in etcd-main volume claims.</p>
</td>
</tr>
</tbody>
</table>
<hr/>
<p><em>
Generated with <a href="https://github.com/ahmetb/gen-crd-api-reference-docs">gen-crd-api-reference-docs</a>
</em></p>
