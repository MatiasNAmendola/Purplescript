# Purplescript #


Purplescript es un lenguaje parecido a ruby escrito en Python que compila PHP.


## Sintaxis ##


### Variables  

	/* PHP */
	$var1 = 'Ejemplo';


	/* Purplescript */
	var1 = 'Ejemplo'



### Constantes

	/* PHP */
	define('PRUEBA', 'constante');

	/* Purplescript */
	PRUEBA = 'constante'


### Material orientado a objetos
	
	
	/* PHP */
	$this->algo->otra_cosa = 'contenido';



	/* Purplescript */
	@algo.otra_cosa = 'contenido'


###	Matrices 
	
	/* PHP */
	$store_data = array
	(
		'producto' => $this->input->post('producto'),
		'activo' => $this->input->post('activo'),
	);

	$simple_array = array( 'elemento1', 'elemento2', 'elemento3' );


	/* Purplescript */
	store_data =
	{

		'producto' : @input.post('producto'),
		'activo' : @input.post('activo')

	}

	simple_array = { 'elemento', 'elemento2', 'elemento3' }





### Flujos de control 
	
	
	/* Purplescript */
	for key, value in store

		echo key

	endfor


	if(expresión)

	elseif(expresión)

	else

	endif





### Funciones 
	
	
	/* PHP */
	function Ejemplo()
	{
		parent::Controller();
		$this->load->model('parent');

	}

	function agregar_producto()
	{

		$this->data['store'] = $this->stores_model->get_store_by_id(store_id);


	}


	/* Purplescript */
	def Ejemplo()

		parent::My_controller()
		@load.model('parent')


	end

	def agregar_producto()

		@data['store'] = @stores_model.get_store_by_id(store_id)

	end
	
	
### CLASSES 
	

    	class Ejemplo extends Controller
	endclass
