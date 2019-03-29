<?php
namespace Sputnik\CoreBundle\Service;

use Symfony\Component\DependencyInjection\ParameterBag\ParameterBagInterface;
use Symfony\Component\Filesystem\Filesystem;

/**
 * Class CacheManager
 *
 * @package App\Service
 */
class CacheManager
{
    /**
     * @var $params ParameterBagInterface
     */
    private $params;

    public function __construct(ParameterBagInterface $params)
    {
        $this->params = $params;
    }

    public function clearCache()
    {

        $fs = new Filesystem();
        $fs->remove($this->params->get('kernel.cache_dir'));
    }

}
